<h1>Filter a SQL query</h1>


<h2>Description</h2>
In this lab activity, you’ll apply basic filters to SQL queries to retrieve information from a MariaDB database.

<h2>Environments Used </h2>

- <b>MariaDB shell</b>

<h2>Scenario:</h2>

In this scenario, you need to get specific information about employees, their machines, and the departments they’re in. Your team needs this data to perform various tasks, such as running updates, posting a privacy notice in certain departments, and sending an alert to an employee with an issue on a machine.

You are responsible for finding the required information by querying a database. You’ll add filters to your queries to locate the information more quickly.

Here’s how you’ll do this task: 

<b>First</b>, you’ll list all organization machines and their operating systems. 

<b>Second</b>, you’ll list all machines with the operating system OS 2. 

<b>Third</b>, you’ll list all the employees in the Finance and Sales departments. Fourth, you’ll obtain information about machines.


<h2>Tutorial walk-through:</h2>

<h3>Task 1. List all organization machines</h3>

In this task, you need to get a list of all organization machines and their operating systems. The data is contained in the machines table. You’ll need to use the SELECT keyword to return specific columns.

Run a SQL query to retrieve only the device_id and operating_system columns from the machines table.

<img src="https://i.imgur.com/JFFneyp.png" height="80%" width="80%"/>

<h3>Task 2. Retrieve a list of the machines with OS 2</h3>

In this task, you need to obtain a list of all machines with the 'OS 2' operating system because these machines need an update. To get this information, you’ll run your first SQL query with a filter.

Select all the records from the machines table with a value of 'OS 2' in the operating_system column. Replace the value X with the correct string:

<img src="https://i.imgur.com/hQ8XKVQ.png" height="80%" width="80%"/>

<h3>Task 3. List employees in specific departments</h3>

In this task, you need to retrieve a list of all the employees in the Finance and Sales departments to obtain their office numbers. A notice about handling confidential financial information will be posted to these offices.

1. Filter the rows returned from department column in the employees table to include only employees from the 'Finance' department. Replace X with the appropriate column name and Y with the appropriate value to complete the filter:

<img src="https://i.imgur.com/vwEEwsN.png" height="80%" width="80%"/>

2. Modify the previous query so that it returns employees who are in the 'Sales' department.

<img src="https://i.imgur.com/kqYCnnW.png" height="80%" width="80%"/>  


<h3>Task 4. Identify employee machines</h3>

Your team recently discovered that there are issues with machines in the South building. In this task, you need to obtain certain employee and computer information.

A machine in 'South-109' has an issue. You need to determine which employee uses that computer so you can send them an alert.

1. Write a query to identify which employee uses the office in 'South-109'. (The data must be returned from the office column in the employees table.)

<img src="https://i.imgur.com/ufc3PVD.png" height="80%" width="80%"/>  

Next, your team has determined that there is an issue with all the machines in the South building. Offices in the organization are named with the building name, a hyphen, and the office number in that building (for example, 'South-109').

2. Modify the query you used in the previous step so that it returns information on all the employees in the 'South' building. Use the LIKE operator with % in this query.

<img src="https://i.imgur.com/g5EMZ9g.png" height="80%" width="80%"/>


<h2>Conclusion</h2>

You now have practical experience in using SQL to

- apply the WHERE clause to filter what a SQL query returns
- use the LIKE operator to filter for patterns

  
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
