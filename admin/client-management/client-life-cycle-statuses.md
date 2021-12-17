# Client Life Cycle Statuses

This page details the Client Life Cycle Statuses and the transitions between the various statuses.

![](https://mifosforge.jira.com/wiki/download/thumbnails/89718816/client%20life%20cycle%20state%20digram.jpg?version=1\&modificationDate=1427539171834\&cacheVersion=1\&api=v2\&width=645\&height=362)

| Action              | State                |
| ------------------- | -------------------- |
| Create client       | Pending for approval |
| Activate            | Active               |
| Close               | Closed               |
| Reject              | Rejected             |
| Withdrawn by client | Withdrawn            |
| Delete              | Deleted              |
| Reactivate          | Active               |

&#x20;On creating a new client, it moves into the  "Pending for approval" state. From the approval state, it can undergo the following transitions:

* On clicking on "Activate", the client gets "Active".\
  **OR**
* On clicking on "Close", the client gets "Closed".\
  **OR**
* On clicking on "Reject", the client gets "Rejected".\
  **OR**
* On clicking on "Withdrawn by client", the client gets "Withdrawn".\
  **OR**
* On clicking on "Delete" the client gets "Deleted". Once a client gets deleted, it won't show up anywhere in LMS.\
  \

* If the client is in the "Closed" state, it can be "Reactivated" to make it "Active".
* If the client is in the following states: Rejected/Withdrawn/Deleted, it cannot be Activated again.&#x20;

{% hint style="info" %}
For the actions mentioned below, we need to update reasons as mentioned below in the Code Values (for more information, navigate to **Admin** >> **System** >> [**Code**](../administration/system/manage-codes.md))
{% endhint %}

| Action   | Reason                   |
| -------- | ------------------------ |
| Close    | Client closure reason    |
| Withdraw | Client withdrawal reason |
| Reject   | Client Rejection reason  |
