# Loan Accounts

#### About Loan Accounts <a href="#loanaccounts-aboutloanaccounts" id="loanaccounts-aboutloanaccounts"></a>

A loan account is an instance of a loan product. A loan account has a unique account number, a specified interest rate, and it is owned by one and only one client or group.&#x20;

A loan account can be created for an active **** client or group based on a loan product that is active on the submitted date. When a loan account is created, it inherits the rules and defaults from the loan product. Your financial institution may allow some of the inherited information to be modified for a loan account depending on how the loan product is defined.



The loan account lifecycle is illustrated in the LMS Loan Account Lifecycle diagram. Loan account statuses are visually indicated in LMS using the colour scheme illustrated in the LMS Loan Account Lifecycle diagram.

![](<../../.gitbook/assets/loan life cycle.png>)

**Figure LMS Loan Account Lifecycle**

The loan account actions/transactions availability and affect on the loan account life cycle status are:&#x20;

| Previous status  | Action/Transaction     | Resulting status                                                                                                                               |
| ---------------- | ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| N/A              | Add Loan               | Pending Approval                                                                                                                               |
| Pending Approval | Add Loan Charge        | Pending Approval                                                                                                                               |
|                  | Approve                | Approved                                                                                                                                       |
|                  | Modify Application     | Pending Approval                                                                                                                               |
|                  | Reject                 | Cancel (Rejected)                                                                                                                              |
|                  | Assign Loan Officer    | Pending Approval                                                                                                                               |
|                  | Withdrawn by client    | Cancel (Withdrawn)                                                                                                                             |
|                  | Delete                 | N/A                                                                                                                                            |
|                  | Add Collateral         | Pending Approval                                                                                                                               |
|                  | Guarantor              | Pending Approval                                                                                                                               |
| Approved         | Assign Loan Officer    | Approved                                                                                                                                       |
|                  | Disburse               | Active                                                                                                                                         |
|                  | Disburse to Savings    | Active                                                                                                                                         |
|                  | Undo Approval          | Pending Approval                                                                                                                               |
|                  | Add Loan Charge        | Approved                                                                                                                                       |
|                  | Guarantor              | Approved                                                                                                                                       |
| Active           | Add Loan Charge        | Active                                                                                                                                         |
|                  | Prepay Loan            | <p>Active if balance owing is greater than zero</p><p>Inactive (Obligation Met) or Closed (Overpaid) if balance is equal or less than zero</p> |
|                  | Make Repayment         | <p>Active if balance owing is greater than zero</p><p>Closed (Obligation Met) or Closed (Overpaid) if balance is equal or less than zero</p>   |
|                  | Undo Disbursal         | Approved                                                                                                                                       |
|                  | Waive Interest         | Active                                                                                                                                         |
|                  | Write-Off              | Closed (Written Off)                                                                                                                           |
|                  | Close (as Rescheduled) | Closed (Rescheduled)                                                                                                                           |
|                  | Close                  | Closed (Obligation Met) or Closed (Overpaid)                                                                                                   |

