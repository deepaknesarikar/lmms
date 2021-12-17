# Teller / Cashier Management

LMS allows an organization to set up cash drawers for proper cash management and reconciliation.

From the Dashboard screen, click on **Admin** then **Organization** from the drop down list. This will launch the [**Organization**](./) menu.

Select **Teller/Cashier Management**

![](../../../.gitbook/assets/teller.png)

{% hint style="info" %}
Before setting up tellers, check the Financial Activity Mappings located under **Accounting** and then map the main cash account to the bank account as well as map the cash at tellers GL to the change fund GL.
{% endhint %}

## **Add Financial Activity Mapping**

Select **Accounting** from the main tab and then select **Accounts Linked to Financial Activities**

![](../../../.gitbook/assets/Screenshot158.png)

This opens a page that displays the financial Activity of an account and the Account name.

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/defineNewMapping.png?version=1\&modificationDate=1552901552260\&cacheVersion=1\&api=v2)

Click on the blue **Define New Mapping** button at the top-right to add a financial activity mapping.

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/addMapping.png?version=1\&modificationDate=1552901763217\&cacheVersion=1\&api=v2)

For Financial activity, select **Cash at Tellers/Cashiers** from the Asset Transfer drop-down list. Also select the Account whose financial activity you want to map.

Click the **Submit** button.

## **Add Teller**

See the [**first**](https://mifosforge.jira.com/wiki/pages/resumedraft.action?draftId=86114424) section to navigate to to the **Teller/Cashier Management** page.

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/tellers.png?version=1\&modificationDate=1552903236766\&cacheVersion=1\&api=v2)

A list of current tellers is displayed with their branch, status and start date. To add a teller, click on the blue **+New Teller** button at the top-right.&#x20;

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/createTeller.png?version=1\&modificationDate=1552903386977\&cacheVersion=1\&api=v2)

Provide Teller details with dates and also ensure to select status as "Active" in-case you want to enable that. Otherwise you could disable it by selecting "In-active".

Click the **Submit** button.

## **Add a new Cashier for Teller**

On Tellers page, select a Teller. This will display an empty list if the teller was not assigned a cashier.

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/selectTeller.png?version=1\&modificationDate=1552903929531\&cacheVersion=1\&api=v2)

Click on the **+ New Cashier For Teller** button on the top-right.&#x20;

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/newCashierforTeller.png?version=1\&modificationDate=1552904103463\&cacheVersion=1\&api=v2)

Select the Cashier or Staff member you want to assign to that teller. This cashier should have been defined in the [Manage Employees](manage-employees.md) section.

Provide the dates within which the cashier is assigned to the teller.

Click on **Submit** button.&#x20;

## **Edit Cashier**

Select the ![](https://mifosforge.jira.com/wiki/download/thumbnails/86114424/viewCashierIcon.png?version=1\&modificationDate=1552913597969\&cacheVersion=1\&api=v2\&width=30\&height=25) button on the Cashier page. This will display the details of the Cashier.

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/editCashier.png?version=1\&modificationDate=1552913713419\&cacheVersion=1\&api=v2)

Select the **Edit** Button at the top-right which will display a page that will permit you to edit.

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/editCashierPage.png?version=1\&modificationDate=1552914003990\&cacheVersion=1\&api=v2)

After editing, click the **Submit** button.

## **View Teller transactions**

&#x20;On Tellers page, select a Teller. This will display details of the teller such as the cashiers who worked on that teller and the period they worked.

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/tellerDetails.png?version=1\&modificationDate=1552910942325\&cacheVersion=1\&api=v2)

Click the first blue button to be able to view the transactions of that cashier.

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/cashierExample.png?version=1\&modificationDate=1552910619992\&cacheVersion=1\&api=v2)

This will display the details of transactions that occurred under that cashier.&#x20;

## **Allocating Cash**

Select the ![](https://mifosforge.jira.com/wiki/download/thumbnails/86114424/allocateCashIcon.png?version=1\&modificationDate=1552911961769\&cacheVersion=1\&api=v2\&width=100\&height=27) button from the **Cashiers** page and this will display the Allocate Cash page.&#x20;

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/allocatingCash.png?version=1\&modificationDate=1552911843035\&cacheVersion=1\&api=v2)

Select date and currency, and provide amount value and notes.

Click the **Allocate Cash** button to submit.

## **Settling Cash**

Select the ![](https://mifosforge.jira.com/wiki/download/thumbnails/86114424/settleCashIcon.png?version=1\&modificationDate=1552912496217\&cacheVersion=1\&api=v2\&width=100\&height=31) button from the **Cashiers** page which will display the Settle Cash Page.

![](https://mifosforge.jira.com/wiki/download/attachments/86114424/settleCashPage.png?version=1\&modificationDate=1552912409010\&cacheVersion=1\&api=v2)

Select the date and currency, and provide the amount and notes on the Settle Cash page.

Click the **Settle Cash** button
