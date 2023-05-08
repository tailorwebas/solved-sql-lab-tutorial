Download Link: https://assignmentchef.com/product/solved-sql-lab-tutorial
<br>
<strong>Lab Objective</strong>

This lab will allow you to use SQL Server Management Studio to create queries in a database. This software allows you to interact with the database directly. This tool allows a Database Administrator to manage and maintain the database.

<strong>Required Materials</strong>

<ul>

 <li>SQL Server 2008 (express or full version).</li>

 <li>AdventureWorks database file</li>

 <li>SQL Lab – Tutorial (this document)</li>

</ul>

<strong>Lab Steps</strong>

<ol>

 <li>Click start, navigate to all programs and select Microsoft SQL Server 2008, and then click on SQL Server Management Studio.</li>

</ol>




<ol start="2">

 <li>Attach the AdventureWorks database to SQL Server 2008.</li>

</ol>




<ol start="3">

 <li>You will now create the following queries using Microsoft SQL Server 2008. For each query create a screenshot to show your results.</li>

</ol>




<ol start="4">

 <li><strong>Query 1</strong> –</li>

</ol>

**** select ALL fields

Select<strong>  *</strong>

from HumanResources.Employee




Insert screenshot below:







<ol start="5">

 <li><strong>Query 2</strong>–</li>

</ol>

***Note ManagerID is NULL***

select EmployeeID, ContactID, ManagerID, HireDate, SalariedFlag

from HumanResources.Employee

<strong>where EmployeeID = 109     </strong>




Insert screenshot below:







<ol start="6">

 <li><strong>Query 3</strong>–</li>

</ol>

*** Use “like” to search for data that matches pattern

**** % is wild card in SQL Server ****”and” specifies that both conditions must be true

select FirstName, LastName, Phone

from Person.Contact

where LastName <strong>like</strong> ‘Mo<strong>%</strong>‘

<strong>and </strong>FirstName <strong>like</strong> ‘G<strong>%</strong>‘

order by LastName




Insert screenshot below:







<ol start="7">

 <li><strong>Query 4</strong>–</li>

</ol>

**** Perform calculations in Select clause

select ProductID, OrderQty, UnitPrice, <strong>OrderQty*UnitPrice as [Extended Price]</strong>, LineTotal

from Sales.SalesOrderDetail

where <strong>OrderQty*UnitPrice &gt; 20000</strong>




Insert screenshot below:







<ol start="8">

 <li><strong>Query 5</strong>–</li>

</ol>

**** select specific row(s)

select EmployeeID, ContactID, ManagerID, HireDate, SalariedFlag

from HumanResources.Employee

<strong>where EmployeeID = 108</strong>




Insert screenshot below:







<ol start="9">

 <li><strong>Query 6</strong>–</li>

</ol>

**** compare dates

select EmployeeID, ContactID, ManagerID, HireDate, SalariedFlag

from HumanResources.Employee

<strong>where HireDate &gt; ‘2002-01-01’</strong>




Insert screenshot below:







<ul>

 <li>Now submit the file with your screenshots to the dropbox.</li>

</ul>





