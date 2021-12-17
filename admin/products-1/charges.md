---
description: Charges are essential part of LMS
---

# Charges

It supports Loan charges and Client Charges.&#x20;

Beginning at the main screen, select **Admin**, **Products** from the drop-down menu. This will launch the **Products** menu. Select **Charges**.

![](../../.gitbook/assets/Screenshot12.png)

## **Creating a Charge**

Click on **+Create Charge**.

![](../../.gitbook/assets/Screenshot13.png)

### **Loan charge**&#x20;

**1.**Select **Charges apply** to as **Loan**.&#x20;

![](<../../.gitbook/assets/Screenshot from 2019-06-12 19-06-14.png>)

2\. Fill in the charge fields described in the **Charge Fields table** below.

3\. Select **Charge time type**&#x20;

![](<../../.gitbook/assets/Screenshot from 2020-07-22 11-44-53.png>)

* **Disbursement**: Gets charged at the time of loan disbursement. You can choose to net-off this amount or collect seperately at product level configurations
* **Specified due date**: Charges can be added at any date in the loan life cycle or can be future dated as well.&#x20;
* **Installment Fee**: Gets charged on every loan installment
* **Overdue Fees**: Gets charged if there is an overdue, this is a **penalty** charge.&#x20;
* **Tranche Disbursement**: Gets charged for Tranche loan disbursement. This is only applicable for the Constant EMI tranche disbursement
* **Top Up**: Charge gets added if you are giving a top-up loan on the existing parent loan
* **Incremental EMI tranche disbursement**. This charge will be collected at disbursment of each tranche
* **Foreclosure Fee**: This charge gets applied at the time of foreclosing the loan
* **ACH bounce fee**: This charge gets added automatically when any ACH is bounced
* **PDC bounce fee**: This charge gets added automatically when any PDC (cheque) is bounced

4\. Select **Charge Calculation**

![](<../../.gitbook/assets/Screenshot from 2020-07-16 13-28-34.png>)

* **Flat:** It is a flat charge.&#x20;
* **% Approved Amount:** $$Approved Amount * Percentage of charge$$&#x20;
* **% Loan Amount + Interest:** $$EMI * percentage charge$$&#x20;
* **% Interest:** $$EMI Interest * Charge Percentage$$&#x20;
* **% Of TopUp Amount :** $$Topup Loan Amount * Percentage Charge$$&#x20;

5\. Select **Charge payment By**

![](<../../.gitbook/assets/Screenshot from 2020-07-16 13-30-21.png>)

Select Regular Mode

6\. Select **Active:**&#x20;

Keep this flag ticked

7\. Select **Tax Group**&#x20;

To create Tax group, you need to create [Tax component](taxation.md#create-tax-components) and [Tax groups](taxation.md#create-tax-group) first

8\. Click **Submit**.

## View Charges

![](../../.gitbook/assets/editcharge.png)

## View / Edit Charges

![](<../../.gitbook/assets/view charge.png>)
