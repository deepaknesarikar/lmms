# Collections

## ACH Collection State Diagram

![](<../../.gitbook/assets/Screenshot from 2020-08-04 15-10-27.png>)

Collection has different state they are as follows

1. Not Registered - This is the initial state where the transaction is not registered
2. Registered - The Transaction is registered
3. Demand Generated - Demand generated means the payment for the particular month is generated, this state of collection can go to Cleared state that is the payment is done received. it can be failed or go into bounce state, From these state i,e bounce and failed the can be generated again as we can see in the above image
4. Cleared - this state states that the payment made by customer is cleared
5. Bounce - generated Demand can be bounce due to any reasons then demand has to be generated again
6. Failed -  payment made by customer is failed will go into this state and lender has to generate the demand again
7. Swapped -&#x20;



## PDC LifeCycle

![](<../../.gitbook/assets/Screenshot from 2020-08-04 16-41-00.png>)

{% hint style="warning" %}
The states are handled in back-end and can not be seen from the UI
{% endhint %}



