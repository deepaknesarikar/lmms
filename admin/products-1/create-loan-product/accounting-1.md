# Accounting

## Product Accounting&#x20;

![](<../../../.gitbook/assets/Screenshot from 2020-07-15 17-31-06 (1).png>)

**By default Accounting will be disabled - None:-** Meaning If you are using this product for various transactions like disbursement, repayment etc. These transactions are not passed in journal entry. &#x20;

**Enabling accounting for the loan product**:-

* To enable Accounting, you need to select either one of the account type below, depending upon your organization accounting practice. &#x20;
  * Cash&#x20;
  * Accrual (periodic)&#x20;
  * Accrual (upfront)&#x20;

![](<../../../.gitbook/assets/image (9).webp>)



| **Field Name (attribute)**      | **Description**                                                                                                                                                                                                                              |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Assets**                      |                                                                                                                                                                                                                                              |
| Fund source                     | <p>An Asset account (typically Bank or Cash) that is debited during repayments/payments and credited using disbursal.</p><p> Applicable to Cash, Accrual (periodic), Accrual (upfront)</p>                                                   |
| Loan portfolio                  | <p>An Asset account that is debited during disbursement and credited during principal repayment/write-off.</p><p> Applicable to Cash, Accrual (periodic), Accrual (upfront)</p>                                                              |
| Interest Receivable             | <p>An Asset account that is used to accrue interest.</p><p> Applicable to Accrual (periodic), Accrual (upfront)</p>                                                                                                                          |
| Fees Receivable                 | <p>An Asset account that is used to accrue fees.</p><p> Applicable to Accrual (periodic), Accrual (upfront)</p>                                                                                                                              |
| Penalties Receivable            | <p>An Asset account that is used to accrue penalties.</p><p> Applicable to Accrual (periodic), Accrual (upfront)</p>                                                                                                                         |
| Transfer in suspense            | An Asset account that is used as a suspense account for tracking portfolios of loans under transfer.                                                                                                                                         |
| **Income**                      |                                                                                                                                                                                                                                              |
| Income from interest            | <p>An Income account that is credited during repayment.</p><p> Applicable to Cash, Accrual (periodic), Accrual (upfront)</p>                                                                                                                 |
| Income from fees                | <p>An Income account that is credited when a fee is paid by account holder on this account.</p><p> Applicable to Cash, Accrual (periodic), Accrual (upfront)</p>                                                                             |
| Income from penalties           | <p>An Income account which is credited when a penalty is paid by account holder on this account.</p><p> Applicable to Cash, Accrual (periodic), Accrual (upfront)</p>                                                                        |
| Income from Recovery Repayments | <p>An Income Account that is credited during recovery repayments</p><p> Applicable to Cash, Accrual (periodic), Accrual (upfront)</p>                                                                                                        |
| **Expenses**                    |                                                                                                                                                                                                                                              |
| Loses written off               | <p>An Expense account that is debited on principal write-off (also debited in the events of interest, fee and penalty written-off in case of accrual based accounting).</p><p> Applicable to Cash, Accrual (periodic), Accrual (upfront)</p> |
| **Liabilities**                 |                                                                                                                                                                                                                                              |
| Overpayment liability           | <p>A Liability account that is credited on overpayments and credited when refunds are made to client.</p><p> Applicable to Cash, Accrual (periodic), Accrual (upfront)</p>                                                                   |
| ****                            |                                                                                                                                                                                                                                              |

## **Advanced Accounting Rule**&#x20;

On clicking on the show button, it enables Advanced accounting rule.

![](<../../../.gitbook/assets/Screenshot from 2020-07-15 17-36-32 (1).png>)

![](<../../../.gitbook/assets/Screenshot from 2020-07-15 17-36-51 (1).png>)

If you click on Add button, it will expand and show up selection drop-downs.&#x20;

* Configure Fund sources for Payment Channels. \
  Example: In the shown image above, Payment type - Cheque is mapped to Fund source - Bank. So whenever payment type is used for transaction, journal entry for Account - Bank will be passed.&#x20;
* Map Fees to Income Accounts.&#x20;
* Map Penalties to Specific Income Accounts. For Reference -[Accounting](broken-reference)

**Click on Submit button to Save/Create loan product.**

![](<../../../.gitbook/assets/image (10).webp>)

### &#x20;<a href="#loanproducts-viewloanproduct" id="loanproducts-viewloanproduct"></a>

| **Accounting Section**                                                                                                                                                                                                                                                                        |                                                                                                                                                                                                                                                                                                                       |   |   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | - | - |
| Accounting                                                                                                                                                                                                                                                                                    | <p>Select one from:</p><ul><li>None</li><li>Cash</li><li>Accrual (periodic)</li><li>Accrual (up front</li></ul><p>If Cash, Accrual (periodic), or Accrual (up front) is selected, see <a href="https://mifosforge.jira.com/wiki/spaces/docs/pages/71565557/Accounting+Loan+Product+Fields">additional fields</a>.</p> |   |   |
| <p><strong>Advanced accounting rules (optional)</strong></p><p> The advanced accounting rules allow for finer detail in mapping payment types to fund sources, fees to income accounts and penalties to income accounts.</p><p> Applicable to Cash, Accrual (periodic), Accrual (upfront)</p> |                                                                                                                                                                                                                                                                                                                       |   |   |
| <p>Configure Fund Sources for Payment Channels</p><p> Payment Type</p><p> Fund Source</p>                                                                                                                                                                                                     | <p>A different Fund Source for each Payment Channel may be specified.</p><p> Select a Payment Type from the <strong>Payment Type</strong> list (e.g.,Cash, check, m-pesa, etc).</p><p> Select a Fund Source from the <strong>Fund Source</strong> list.</p>                                                           |   |   |
| <p> Map Fees to Income Accounts</p><p> Fees</p><p> Income Account</p>                                                                                                                                                                                                                         | <p>A different Income Account for each Fee type may be specified.</p><p> Select a Fee from the <strong>Fee</strong> list.</p><p> Select an Income Account from the <strong>Income Account</strong> list.</p>                                                                                                          |   |   |
| <p>Map Penalties to Specific Income Accounts</p><p> Penalty</p><p> Income Account</p>                                                                                                                                                                                                         | <p>A different Income Account for each Penalty type may be specified.</p><p> Select a Penalty from the <strong>Penalty</strong> list.</p><p> Select an Income Account from the <strong>Income Account</strong> list.</p>                                                                                              |   |   |
