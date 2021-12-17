# Product Mix

The **Product Mix** function allows a financial institution to define rules that restrict the loan accounts that may be held by a client at once. LMS checks a client's active loan accounts when a new loan is being disbursed. If there is a conflict between the client's active loan accounts and the loan account to be disbursed, it will result in an error and the new loan account will not be disbursed.&#x20;

By default, the system does not restrict any product combinations.

From the Dashboard, select **Admin**, then **Products** from the drop-down menu.

![](<../../.gitbook/assets/Screenshot from 2020-07-22 11-52-09.png>)

This will launch the **Products** menu.\
Select **Product Mix.**&#x20;

![](../../.gitbook/assets/Screenshot15.png)

## **Creating a new Product Mix**

1. Navigate to **Admin** >> **Products** and click on '**Product Mix**' to see the following window:

![](<../../.gitbook/assets/Screenshot16 (1).png>)

1. Click on '**+Add**' ![](https://mifosforge.jira.com/wiki/download/thumbnails/103186467/image2019-4-22\_1-58-24.png?version=1\&modificationDate=1555878505396\&cacheVersion=1\&api=v2\&width=50\&height=28) button, and the following window will be displayed:\

2. Select the loan product from the drop-down menu (_for instance: Agriculture_). After choosing the loan product, you can decide which loan products a client can get (_Allowed Products_) and which loan products are prohibited for the client (_Restricted Products_). \


![](<../../.gitbook/assets/Screenshot from 2020-07-22 11-59-41.png>)



* Move loan products from the **Allowed Products** list to the **Restricted Products** list by clicking on the product name and clicking on **>>**.
* Move loan products from the **Restricted Products** list to the **Allowed Products** list by clicking on the product name and clicking on **<<**.

![](../../.gitbook/assets/editprodmix.png)

1. Once you're done, click on the '**Submit**' button ![](https://mifosforge.jira.com/wiki/download/thumbnails/103186467/image2019-4-22\_2-2-33.png?version=1\&modificationDate=1555878754331\&cacheVersion=1\&api=v2\&width=55\&height=26) to create a product mix.&#x20;

{% hint style="info" %}
For example: if you have three different loan products (A, B, and C), you can make a rule that if a client has taken loan A, then the client can have loan B but not C.&#x20;
{% endhint %}

## **Edit or Delete Product Mix**

1. To edit or delete a Product Mix, navigate to **Admin** >> **Products** >> **Product Mix.** The following window will be displayed: \
   \
   ![](https://mifosforge.jira.com/wiki/download/thumbnails/103186467/Capture%2018.PNG?version=1\&modificationDate=1484283575779\&cacheVersion=1\&api=v2\&width=1080\&height=523)\
   \

2. Click on the loan product on which the Product Mix is defined (_in this example, 'Agricultural Loan'_) to view the Product Mix:\
   \
   ![](https://mifosforge.jira.com/wiki/download/thumbnails/103186467/Capture%2017.PNG?version=2\&modificationDate=1484283633560\&cacheVersion=1\&api=v2\&width=1080\&height=565)\
   \

3. Either click on '**Edit**' or the '**Delete**' button to modify or delete the product mix respectively.
