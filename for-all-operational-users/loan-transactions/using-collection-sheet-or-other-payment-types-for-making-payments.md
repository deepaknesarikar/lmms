# Using collection sheet or other payment types for making payments

## Using collection sheet or other payment types for making payments <a href="#title-text" id="title-text"></a>

This section describes the steps to record a repayment on a JLG loan account. The following methods are available:

* collection sheet&#x20;
* repayment via cash or similar payment type
* one time transfer from saving account
* standing instruction transfer from saving account\


For repayments of client loan accounts see [How to Make Repayments on a Client Loan Account](how-to-make-repayments-on-a-client-loan-account.md) For repayments of group loan accounts see [How to Make Repayments on a Group Loan Account](how-to-make-repayments-on-a-group-loan-account.md)



**Tip: It's mandatory to attach meeting in order to use collection sheet.** Attaching meeting at Center [Manage Centers](../../admin/client-management/manage-centers.md) Attaching meeting at Group [Manage Groups](../../admin/client-management/manage-groups.md)

#### To make a repayment using the collection sheet (and productive collection sheet) <a href="#usingcollectionsheetorotherpaymenttypesformakingpayments-tomakearepaymentusingthecollectionsheet-and" id="usingcollectionsheetorotherpaymenttypesformakingpayments-tomakearepaymentusingthecollectionsheet-and"></a>

The collection sheet is a way to create bulk transactions for repayment of loans You can use collection sheet in two ways.

* Using it as a Productive Collection Sheet where you have to provide three parameters, namely: Office, Meeting Date and Staff & later you can chose respective centers before submission.
* Using it as just a 'Collection Sheet' where you can provide Office, Meeting Date, Staff and Center. Providing 'Group Name' is optional here.&#x20;

#### Using Productive Collection Sheet: <a href="#usingcollectionsheetorotherpaymenttypesformakingpayments-usingproductivecollectionsheet" id="usingcollectionsheetorotherpaymenttypesformakingpayments-usingproductivecollectionsheet"></a>

* Go to the left panel and click on 'Collection Sheet'.

![](<../../.gitbook/assets/Screenshot from 2020-07-22 14-09-49.png>)

The following window appears. Provide office name, meeting date and staff.

![](<../../.gitbook/assets/Screenshot from 2020-07-22 14-09-49 (1).png>)

Click on 'Productive Collection Sheet' to see the following window where you can select the center (the selected center is shown with Amber color). It also shows Branch Office Name, Meeting Date and center total collection for the given meeting date in terms of loan product. Here, 16200 is the collection for one loan product and 321 is the collection for another loan product.

![](<../../.gitbook/assets/image (101).png>)

Click on ![](https://mifosforge.jira.com/wiki/download/thumbnails/72909396/d4.jpg?version=1\&modificationDate=1415957389473\&cacheVersion=1\&api=v2\&width=30\&height=24) button to see the details of the collection group-wise and client-wise for the selected center as shown below, or you can simply click on 'Submit and Next center' button.&#x20;

![](<../../.gitbook/assets/image (102).png>)



* As you can see, there are two groups and each group has three clients. IGL is the loan product (short name) for the group 'Santa Maria Group 2' and VRL is the loan product for the group 'Santa Maria Group 1'. You can see 'Due' for each client as well as the due for each group and you can also see Attendance where using the drop-down menu, you can select whether the client is present, Absent, Leave, Late and Approved.
* Once you verify all the details are correct, you just click on 'Submit' button.&#x20;

#### Using Collection Sheet: <a href="#usingcollectionsheetorotherpaymenttypesformakingpayments-usingcollectionsheet" id="usingcollectionsheetorotherpaymenttypesformakingpayments-usingcollectionsheet"></a>

Go to the left panel and click on 'Collection Sheet' to see the following window.

![](<../../.gitbook/assets/image (78).webp>)

Provide all the details (Selecting Group is optional. If you select the group, the collection sheet for that group is shown only, otherwise the collection sheet for all the groups for the selected center will be shown) and click on 'Collection Sheet' button to see the following window.

![](<../../.gitbook/assets/image (103).png>)

Just like the previous one, verify the details and click on 'Submit' button. If everything goes fine, You will get the message "Collection Sheet Saved Successfully".

#### Capturing payment details for collection sheet:  <a href="#usingcollectionsheetorotherpaymenttypesformakingpayments-capturingpaymentdetailsforcollectionsheet" id="usingcollectionsheetorotherpaymenttypesformakingpayments-capturingpaymentdetailsforcollectionsheet"></a>

Step 1) Define payment types in Admin >> Organization >> Payment type, as shown in the screen shot below.

![](<../../.gitbook/assets/image (80).webp>)

Step 2) Click on collection sheet:&#x20;

a - Select "Branch office",&#x20;

b - Select Date - "Meeting calendar"&#x20;

c - Select "Staff"&#x20;

d - Select "Center"&#x20;

e - If required select "Group" Click on "Collection sheet"

![](<../../.gitbook/assets/image (81).webp>)

Step 3) Once the collection sheet gets generated, at the bottom you would find: "Add payment type" button - Click on it.

![](<../../.gitbook/assets/image (82).webp>)

Step 4) In Payment type: By Inputting the required fields you can capture details i.e Payment type, Account #, Receipt #, etc

![](<../../.gitbook/assets/image (83).webp>)

#### To make a repayment using cash or similar payment type <a href="#usingcollectionsheetorotherpaymenttypesformakingpayments-tomakearepaymentusingcashorsimilarpaymentty" id="usingcollectionsheetorotherpaymenttypesformakingpayments-tomakearepaymentusingcashorsimilarpaymentty"></a>

Locate the loan account by navigating to it through the client who holds the loan account.

1. Select **Make Repayment** from the action bar.
2. Accept the default **Transaction date** or select a different date from the calendar pop-up.
3. Accept the default **Transaction amount** or type a different repayment amount.
4. Select **Payment type** from the list.
5. Click **+** to add payment details (optional).
   1. Account#
   2. Check#
   3. Routing code
   4. Receipt#
   5. Bank#
6. Type relevant notes.
7. Click **Submit.**

The loan account repayment will be recorded and the repayment schedule and loan summary will be updated with the payment information.

#### To make loan repayments from a saving account (one time transfer) <a href="#usingcollectionsheetorotherpaymenttypesformakingpayments-tomakeloanrepaymentsfromasavingaccount-onet" id="usingcollectionsheetorotherpaymenttypesformakingpayments-tomakeloanrepaymentsfromasavingaccount-onet"></a>

Locate the saving account from which the loan repayment will be made (the originating account).



1. Click the saving account name in the list to view the saving account information.
2. Click **More** and **Transfer Funds** from the action bar.
3. Select the group and account (the destination loan account to be repaid) to transfer funds to:
   1. **Office**: Select the office where the destination loan account is located.
   2. **Client**: Select the client who holds the destination loan account.&#x20;
   3. **Account type**: Select the loan product type upon which the destination loan account is based.
   4. **Account**: Select the destination loan account.
   5. **Amount**: Type the transfer amount.
4. Select the **Transaction date** from the calendar pop-up.
5. Type any notes in **Description**
6. Click **Submit**.&#x20;

#### To make loan repayments from a saving account (standing instruction transfer) <a href="#usingcollectionsheetorotherpaymenttypesformakingpayments-tomakeloanrepaymentsfromasavingaccount-stan" id="usingcollectionsheetorotherpaymenttypesformakingpayments-tomakeloanrepaymentsfromasavingaccount-stan"></a>

Standing instructions can be set up to transfer funds from a saving account to a loan account. The transfer will take place based on the schedule defined in the standing instruction. For a loan repayment, the standing instruction schedule can be set to match the loan repayment schedule.

Locate the client or group whose savings account will be the origination of the funds for the transfer.

1. Click **More** and **Create standing instructions** to create new standing instructions.
2. Complete the fields on the **Create Standing Instruction** form.
3. Click **Submit**.

The standing instruction will be created and will be in effect from the **Validity from** date until the **To** date inclusive; or until the standing instruction is Disabled.

## &#x20;<a href="#title-text" id="title-text"></a>

