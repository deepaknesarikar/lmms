---
description: >-
  Employees are people within your organization who do not have access to the
  LMS Platform
---

# Manage Employees

**Employees** are people within your organization who do not have access to the LMS system. They are used to distinguish between the various types of staff as well as their roles and permissions (for instance: it designates loan officers and provides the ability to assign a loan officer to a client, group or loan).&#x20;

From the Dashboard, click on the **Admin** button on the top menu bar and click on **Organization** from the drop down list. This will launch the [**Organization**](./) menu.

Select **Manage Employees**.

![](../../../.gitbook/assets/manageemp.png)

A list of all employees will be displayed:

![](../../../.gitbook/assets/emplist.png)

### **Add Employees**

Click the ![](https://mifosforge.jira.com/wiki/download/thumbnails/67141732/createEmployeeButton.png?version=1\&modificationDate=1552739669290\&cacheVersion=1\&api=v2\&width=120\&height=25) button at the top-right of the page to create a new employee.

![](../../../.gitbook/assets/createemployee.png)

1. Fill the following **mandatory** fields (_denoted by a red asterisk "\*"_):
   * Select the appropriate office from the **Office** drop-down menu.
   * Enter the employee's **First name.**
   * Enter the employee's **Last name**.
   * Provide the **Joining Date** of the employee.\

2. Furthermore, fill the following **optional** fields:
   * &#x20;Designate the employee as a loan officer (if required) by checking the "**Is loan officer?**" checkbox.
   * Add a **Mobile Number for SMS** to allow messages via text.

Click on **Submit** once you are done.

### **Import Employee**

You can also import employee details from your local device. Click the ![](https://mifosforge.jira.com/wiki/download/thumbnails/67141732/importEmployeesButton.png?version=1\&modificationDate=1552895754837\&cacheVersion=1\&api=v2\&width=120\&height=26) button at the top-right of the page (_next to the blue Create Employee button_) on the **Manage Employees** page.

This page has three sections (_as shown below_):

* Employee Template
* Import Employees
* Documents

![](https://mifosforge.jira.com/wiki/download/attachments/67141732/import\_employees.PNG?version=1\&modificationDate=1553978991489\&cacheVersion=1\&api=v2)

If you want to use an already existing template, go to the **Employee Template** section.

![](https://mifosforge.jira.com/wiki/download/attachments/67141732/searchAndDownloadTemplate.png?version=1\&modificationDate=1552896092452\&cacheVersion=1\&api=v2)

Select an office template in the **Select Office** drop-down menu. Click the **Download** button to the right of the search field. This will download a spreadsheet file in which you can add employee details. For example: let's assume we selected the **Main Head Office** template and the downloaded spreadsheet includes the following fields:&#x20;

* Office Name
* First Name
* Last Name
* Loan Officer
* Mobile Number
* Joining date
* External Id
* Status

#### ![](https://mifosforge.jira.com/wiki/download/attachments/67141732/employeeTemplate.png?version=1\&modificationDate=1552896512189\&cacheVersion=1\&api=v2) <a href="#manageemployees" id="manageemployees"></a>

Once you have filled the details in the spreadsheet, save it and then import the file into LMS in the **Import Employees** section of the page.

![](https://mifosforge.jira.com/wiki/download/attachments/67141732/chooseAndUploadTemplate.png?version=1\&modificationDate=1552897804327\&cacheVersion=1\&api=v2)

Click the grey **Choose File** button, navigate to where you saved your file, select it and then click the blue **Upload** button to import your employee details.

![](https://mifosforge.jira.com/wiki/download/attachments/67141732/viewUploadedTemplate.png?version=1\&modificationDate=1552897990042\&cacheVersion=1\&api=v2)

In the **Documents** section at the bottom of the page, click the **Refresh** button to confirm that the file has been uploaded and can be used in LMS.

### **View Employees**

Once you have selected **Manage Employees,** a chart of all employees will be displayed with the following information:

* The employee's **Name**
* Whether the employee **Is a Loan Officer** or not
* The employee's **Office**
* The employee's **Status**; whether true or false

![](../../../.gitbook/assets/emplist.png)

{% hint style="info" %}
Use the **Filter by Name** field to quickly locate the employee you are searching for. Begin typing the employee's name and LMS will automatically filter the results.
{% endhint %}

Clicking on an employee's name on the chart will open that employee's **Profile**:

![](https://mifosforge.jira.com/wiki/download/attachments/67141732/employeeProfile.png?version=1\&modificationDate=1552740679411\&cacheVersion=1\&api=v2)

### **Edit Employee**

Click the blue **Edit** button at the top-right of the employee's profile to edit the employee's information. This will launch a new page where you may change the employee's information:

![](https://mifosforge.jira.com/wiki/download/attachments/67141732/editemployee.png?version=2\&modificationDate=1552740755739\&cacheVersion=1\&api=v2)

Once the appropriate changes have been made, click **Submit**.

{% hint style="warning" %}
An employee is not the same as a User (and is not interlinked with Users). Therefore, you may need to create users separately. Please see the [Users](../users.md) section of this manual to learn more. In short, All users are the employees. But all employees may not be the users.&#x20;
{% endhint %}
