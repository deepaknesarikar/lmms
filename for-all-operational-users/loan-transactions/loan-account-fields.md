# Loan Account Fields

## Loan Account Fields



| Field Name (attribute) | Description | Example | Validations (if applicable) |
| ---------------------- | ----------- | ------- | --------------------------- |

| **Details Section** |
| ------------------- |

| Product | <p>Product is the name of the loan product that the loan account is based upon. For a new loan account, the loan account form will be populated with the loan product defaults and rules when the loan product name is selected from the list. Depending on the loan product definition, some fields may or may not be visible on the loan account form.</p><p>Cannot be changed once a loan account is approved.</p> | Home Building Loan A | <p>Required field</p><p>Select from list</p> |
| ------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------- | -------------------------------------------- |

| Loan Officer | Loan officer is the financial institution representative who has responsibility for and interacts with the client/group associated with a loan account. |   | <p>Optional</p><p>Select from list</p> |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- | - | -------------------------------------- |

| Loan Purpose | <p>The loan purpose provides an indication of how the funds provided through the loan will be directed and can be used to group loans with the same purpose for reporting. The values in the list are defined by your system administrator.</p><p>Cannot be changed once a loan account is approved.</p> | Agriculture | <p>Optional</p><p>Select from list</p> |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | -------------------------------------- |

| Fund | <p>The fund value will be filled in from the loan product definition. It may be modified on the loan account if a different fund should be linked to the loan account.</p><p>Cannot be changed once a loan account is approved.</p> |   | <p>Optional</p><p>Blank, default, or select from list</p> |
| ---- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | - | --------------------------------------------------------- |

| Submitted on | <p>The date the loan account application was received. The date may be a date in the past or today's date. It cannot be future-dated. Select the date from the pop-up calendar or enter the date in the prescribed date format.</p><p>Cannot be changed once a loan account is approved.</p> | 01 Jan 2013 | <p>Required field</p><p>Date</p><p>dd mm yyyy</p> |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | ------------------------------------------------- |

| Disbursement on | <p>The date that the loan account is expected to be disbursed.</p><p>Cannot be changed once a loan account is approved.</p> | 08 Jan 2013 | <p>Required field</p><p>Date</p><p>dd mm yyyy</p> |
| --------------- | --------------------------------------------------------------------------------------------------------------------------- | ----------- | ------------------------------------------------- |

| External Id | Provides an external id for the loan account. |   |   |
| ----------- | --------------------------------------------- | - | - |

| <p><strong>Meeting Details (For Group and JLG Loans)</strong></p><p>If the loan account is for a group or JLG and the group has a meeting schedule, loan disbursement and the repayment schedule can be tied to the meeting schedule. The loan account form will display group meeting start date and repeat frequency.</p> |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

| Sync repayments with meeting | Used to sync the scheduled repayment dates with the group's meeting dates. |   | Checked means repayment dates will sync with meeting dates |
| ---------------------------- | -------------------------------------------------------------------------- | - | ---------------------------------------------------------- |

| Sync disbursement date with meeting | Used to schedule loan disbursement on a group meeting date. |   | Checked means loan disbursement will be schedule on a meeting date |
| ----------------------------------- | ----------------------------------------------------------- | - | ------------------------------------------------------------------ |

| **Terms Section** |
| ----------------- |

| Principal | <p>Principal is the amount of money to be loaned. The principal will default to the value set in the loan product. The principal may be modified but must be within any minimum to maximum range specified on the loan product.</p><p>Cannot be changed once a loan account is approved.</p> | 10000 | <p>Required fields</p><p>Numeric</p> |
| --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----- | ------------------------------------ |

| Loan term | <p>The loan term is the length of time the client or group agrees to repay the loan. The loan term will default to the value set in the loan product. The loan term may be modified but must be within any minimum to maximum range specified on the loan product.</p><p>Cannot be changed once a loan account is approved.</p> | 52 Weeks | <p>Required fields</p><p>Numeric and select from list</p> |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- | --------------------------------------------------------- |

| Number of repayments | <p>The number of repayments specifies the number of repayments to be made from the time the loan is disbursed until the financial obligation of the loan is expected to be met. The number of repayments will default to the value set in the loan product. The number of repayments may be modified but must be within any minimum to maximum range specified on the loan product.</p><p>Cannot be changed once a loan account is approved.</p> | 26 | Required fields |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -- | --------------- |

| Repaid every | <p>Repaid every specifies the frequency of repayments. The frequency will default to the value set in the loan product. The frequency may be modified.</p><p>Cannot be changed once a loan account is approved.</p> | 2 Weeks | <p>Required field</p><p>Numeric and select from list</p> |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- | -------------------------------------------------------- |

| First repayment on | <p>A first repayment date may be entered to override the date the system would schedule.</p><p>Cannot be changed once a loan account is approved.</p> | 15 June 2014 | <p>Optional</p><p>Date format DD MM YYYY</p> |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | -------------------------------------------- |

| Interest charged from | <p>An interest charged from date may be entered to override the date the system would start charging interest.</p><p>Cannot be changed once a loan account is approved.</p> | 15 June 2014 | <p>Optional</p><p>Date format DD MM YYYY</p> |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | -------------------------------------------- |

| Nominal interest rate | The nominal interest rate will default from the loan product setting. A loan officer may be able to modify the interest rate but will not be able to modify the interest rate period (e.g., monthly, yearly). | 1.25 yearly | <p>Required field</p><p>Numeric</p> |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | ----------------------------------- |

| Interest method | The interest method will default from the loan product setting. A loan officer may select a different interest method for the loan account. | Flat | <p>Required field</p><p>Select from list</p> |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ---- | -------------------------------------------- |

| Amortization | Amortization will default from the loan product setting. A loan officer may select a different amortization for the loan account. | Equal Installments | <p>Required field</p><p>Select from list</p> |
| ------------ | --------------------------------------------------------------------------------------------------------------------------------- | ------------------ | -------------------------------------------- |

| Interest calculation period | The interest calculation period will default from the loan product setting. A loan officer may select a different interest calculation period for the loan account. | Same as repayment period | <p>Required field</p><p>Select from list</p> |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ | -------------------------------------------- |

| Arrears tolerance | The arrears tolerance will default from the loan product setting. A loan officer may select a different arrears tolerance amount for the loan account. | .01 | <p>Optional field</p><p>Numeric</p> |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | --- | ----------------------------------- |

| Interest free period | The interest free period will default from the loan product setting. A loan officer may select a different interest free period for the loan account. |   | <p>Optional field</p><p>Numeric</p> |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | - | ----------------------------------- |

| Repayment strategy | The repayment strategy will default from the loan product setting. A loan officer may select a different repayment strategy for the loan account. | LMS style | <p>Required field</p><p>Select from list</p> |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------- | --------- | -------------------------------------------- |

| <p>Moratorium</p><p>On principal payment</p><p>On interest payment</p><p>On Arrears Ageing</p> | The moratorium information will default from the loan product settings. A loan officer may select different moratorium values for the loan account. |   | Optional fields |
| ---------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | - | --------------- |

| Link savings | Select a saving account to link to the loan. If there is a saving account linked, the loan funds may be disbursed to the saving account and loan repayments may be transferred from the saving account. The list will be populated with saving accounts that are eligible to link to the loan account. If the list is empty, there are no eligible saving accounts. |   | Select from list |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | - | ---------------- |

| <p><strong>Charges Section</strong></p><p>Charges defined on the loan product will automatically appear as charges on the loan account. Default charges may be removed by clicking the <strong>X</strong> under the <strong>Actions</strong> column. Charges may also be added as described in this section.</p> |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

| Charges | Select a charge from the **Charges** list and click **Add**. If more charges apply to the loan product, select additional charges and click **Add** for each. |   |   |
| ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | - | - |

| Overdue Charges | Select an overdue charge from the **Overdue Charges** list and click **Add**. If more overdue charges apply to the loan product, select additional overdue charges and click **Add** for each. |   |   |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | - | - |

| **Collateral** |
| -------------- |

| <p>Collateral</p><p>Collateral</p><p>Value</p><p>Description</p> | <p>Identify any items the client or group provides as collateral for the loan account.</p><p>Your financial institution will define the <strong>collateral</strong> types it accepts.</p><p><strong>Value</strong> is the value of the collateral item expressed in the same currency as the loan account's currency.</p><p>The <strong>description</strong> is used to provide details of the collateral item.</p><p>Add as many collateral items as desired or available.</p> |   | <p>Optional</p><p>Select from list</p><p>Numeric</p><p>Alphanumeric</p> |
| ---------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | - | ----------------------------------------------------------------------- |

## &#x20;<a href="#title-text" id="title-text"></a>

