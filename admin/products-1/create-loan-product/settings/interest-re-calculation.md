# Interest Re-calculation

## Interest Amount Recalculation for Loan Accounts <a href="#title-text" id="title-text"></a>

![](<../../../../.gitbook/assets/image (6) (1).webp>)

### Overview <a href="#interestamountrecalculationforloanaccounts-overview" id="interestamountrecalculationforloanaccounts-overview"></a>

When repayments are on time and for the exact due amount always, then there is usually no need for interest recalculation.

However, when repayments are either not on time or not for the due amount, then the following scenarios need to be handled:

a) Exact Due Amount is paid and

*
  * is paid Late
  * is paid Early

b) Only part of the Due Amount is paid and:

*
  * is paid On Time
  * is paid Late
  * is paid Early

c) Excess of Due Amount is paid and:

*
  * is paid On Time
  * is paid Late
  * is paid Early

For such scenarios, the exact interest amount calculation depends on following factors:

a) Days Calculation Basis:

* Actual
* 30 – here number of days will be computed as (Y2-Y1)\*360 + (m2-m1)\*30 + (d2-d1)

d1 and d2 will be treated as 30 if they are > 30

b) Number of days in a year:

* Actual
* 360
* 365
* 364

c) Rest or Frequency at which outstanding principal is recalculated – may be daily, weekly, fortnightly or monthly

At the end of every business day a batch job (Loan Interest Recalculation) will kick off which will check all active accounts for which interest recalculation is set to "true". The job then checks if there the interest calculated vs interest specified in repayment schedule matches. If yes,&#x20;

#### Background and strategic fit <a href="#interestamountrecalculationforloanaccounts-backgroundandstrategicfit" id="interestamountrecalculationforloanaccounts-backgroundandstrategicfit"></a>

Many financial institutions have the need to re-compute interest based on actual date of repayment. This feature is a must when LMS needs to support operations of a commercial bank.

#### Requirements/User Stories <a href="#interestamountrecalculationforloanaccounts-requirements-userstories" id="interestamountrecalculationforloanaccounts-requirements-userstories"></a>

| Title               | User Story                                                                                     | Importance | Notes |
| ------------------- | ---------------------------------------------------------------------------------------------- | ---------- | ----- |
| Define Loan Product | As an Operations Manager, I want to define a loan product that supports interest recalculation | Must Have  |       |
| Create Loan Account | As an Loan Officer, I want to create a loan account that supports interest recalculation       | Must Have  |       |

#### Business Rules <a href="#interestamountrecalculationforloanaccounts-businessrules" id="interestamountrecalculationforloanaccounts-businessrules"></a>

A **Daily** Rest may be specified for loans of any frequency and the days in year may be:

* 365 – for all repayment frequency
* 364 – for weekly or fortnightly repayment loans
* 360 – for monthly repayment loans

A **Weekly** Rest may be specified for loans that are repaid weekly or fortnightly and the days in year may be 365 or 364

A **Fortnightly** Rest may be specified for loans that are repaid fortnightly and the days in year may be 365 or 364

A **Monthly** Rest may be specified for loans that are repaid Monthly and the days in year may be 365 or 360

These rules will not be implemented in the LMS code. But this is expected to be followed defining loan products and loan accounts. LMS will be tested only in the above scenarios for consistent interest amount calculations.

Interest Amount Calculation will be done as follows:

Interest = Principal \* Annual Interest Rate \* Days Calculated / Number of Days in a Year

* Principal – Principal as per the Rest Specified
* Days Calculated – based on “Days Calculation Basis”

Other rules that will be followed:

a) When interest recalculation is turned on for a loan product, then any excess amount (over what is currently due or overdue) will be applied to the outstanding principal always. In this respect, it will override the settings for Repayment Strategy selected.

b) Any interest compounding will stop if any amount is overdue more than the number of days for the account to be treated as Non-Performing Asset (overdue\_days\_for\_npa).

c) If there is a disbursement-time fee, which is calculated on principal+interest - then this fee amount will not be recomputed based on interest recalculations.

d) If any interest (or fee) was waived on an account - and the interest (or fee) changes due to the recalculations - then the waived amount will not be automatically changed by LMS.

Example:

&#x20;    Total Interest dues: Apr-14 - 300, May-14 - 250 and Jun-14 - 200

&#x20;    Interest Waived = 300 (i.e. entire Apr-2014's interest is waived)

&#x20;    Due to interest recalculation (due to a back-dated transaction), the interest amounts now change to: Apr-14 - 250, May-14 - 200 and Jun-14 - 150

&#x20;    The waived amount remains as 300 (i.e. April's interest of 250  is waived and from May's interest - 50 is waived. If other behavior is needed, then user has to reverse the earlier waiver and then apply interest recalculation and then re-do the waiving with new amount).

The only situation when LMS will automatically change the waived amount is when the total recalculated interest (or fee) due is less than the waived amount. In such a case, the waived amount is reduced to the recalculated amount.

e) If a fee is already paid and due to the recalculations if the fee is reduced (or increased), then the fee paid transaction is not altered. Any excess fees already paid in can be refunded at the end of the tenure of the loan (as then it will show that the account is overpaid). If there is an increase in fee due to the recalculations, then the additional fee can be collected.

#### Attributes <a href="#interestamountrecalculationforloanaccounts-attributes" id="interestamountrecalculationforloanaccounts-attributes"></a>

For Loan Products and Loan Accounts

(Note: For Loan Accounts – all the below 4 attributes are inherited from Loan Product and cannot be modified for each account)

| Attributes                                               | Description                                                                                                                                                          | Note                                             |
| -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------ |
| Days In Year                                             | <p>Number of days to be considered for a year when calculating interest. Can be:</p><p>Actual</p><p>365</p><p>360</p><p>364</p>                                      | <p>Not Null</p><p>Default is "Actual"</p>        |
| Recalculate Interest?                                    | For this loan product, if interest is to be recalculated when early or late payments or exact amount is not paid (True or false)                                     | <p>Checkbox – Nullable</p><p>Default is Null</p> |
| Frequency at which Outstanding Principal is recalculated | <p>Rest or Frequency at which outstanding principal is recalculated –</p><p>Same as Repayment Frequency</p><p>Daily</p><p>Weekly</p><p>Fortnightly</p><p>Monthly</p> | <p>Dropdown - Nullable</p><p>Default is Null</p> |
| Days Calculation Basis                                   | <p>Basis for calculation of number of days between the start and end dates</p><p>Actual</p><p>30</p>                                                                 | Default is Actual                                |

#### &#x20;<a href="#interestamountrecalculationforloanaccounts-securityandpermissions" id="interestamountrecalculationforloanaccounts-securityandpermissions"></a>

#### New Screens <a href="#interestamountrecalculationforloanaccounts-newscreens" id="interestamountrecalculationforloanaccounts-newscreens"></a>

New Screen will capture "Principal Pre-payment" details. This screen will be similar to "Make Repayment" screen. This screen will used to make a pre-payment on principal.

Fields to be captured:

* Transaction Date
* Principal Prepayment Amount
* Principal Outstanding (Read-only field)
* Interest Outstanding (Read-only field)
* Payment Type
* Payment Details
* Notes

This button will be enabled only for products where "Recalculate Interest?" is set to "true". The future interest is recalculated and repayment schedule is regenerated with revised interest and principal repayments when this screen is submitted. A preview needs to be shown with revised repayment schedule before this screen is submitted.

The older version of the repayment schedule needs to be saved so that it can be viewed, when needed.

#### Use cases: <a href="#interestamountrecalculationforloanaccounts-changestoexistingscreens" id="interestamountrecalculationforloanaccounts-changestoexistingscreens"></a>

&#x20;    1\. **identify  recalculation** : check the payment against schedule and should process recalculation in following scenarios&#x20;

1. late payment, should be identified by a  batch job
2. back dated entry
3. pre-payment
4. on time with advanced-payment / less payment(ex : on 3rd should pay 1000 but the payment is done for 500 or 1500)

&#x20;    2\.  **process recalculation :**

1.
   1. identify outstanding principal&#x20;
   2. identify amount for interest compound&#x20;
   3. regenerate schedule based on outstanding and rest frequency(from calendar instance)
   4. add the extra interest(in-case of late payment ) to next installment
      1. for last installment,  will add extra installments with interest component only&#x20;
   5. if prepayment is done then use one of the strategy to reschedule.
      1. adjust EMI amount &#x20;
      2. adjust loan duration
      3. adjust next installments

&#x20;    3\. Capture new fields for loan product and account(editable only from product level but will maintain a copy at account level)

&#x20;    4\. Add new screen for pre-payment(internally same as repayment but will return recalculated interest by setting closure date as today)

&#x20;    5\. change schedule generator to use newly added days in year and days in month values&#x20;
