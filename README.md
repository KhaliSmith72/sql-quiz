# SQL QUIZ

- What data would be contained in the left join of two tables?
The data that has information that isn't relevant to the right table
- What data would be contained in the right join of two tables?
The data that has information that isn't relevant to the left table
- What data would be contained in the inner join of two tables?
An inner join would display all the data in both tables that contained relevant data.
- What data would be contained in a full join of two tables?
All data in both tables regardless of their key relationships.
- What tool can be used to track all the queries being used by an application?
Sql execution manager
- What tool can be used to analyze a query?
Profile
- Describe CRUD.
C is for creating a database, R is for reading that databases information, U is for updating that database, and D is for deletion of either the whole database, or an item within it.
- What does it mean if a database is ACID compliant?
It means that it works?
- What global variable contains the identity value of the last record inserted into a database?
@@identity
- What function can be used to get the current date and time?
DateTime.Now
- TRUE or FALSE: when a table has a primary key, the value of that column is automatically incremented every time a new record is inserted into that table.
True
- What is a primary key and why do we use them.
A primary key is something we use to set a relationship between to databases.
- What is a foreign key and why do we use them.
Foreign keys do the same, although I don't think they have as much of an impact.
- What is one way to improve the search performance of a table?

- If you are going to perform a series of transactions and you wish to undo the transactions if one fails, what functionality could you use to undo the changes?
Try Catch
Use the following tables for the next questions:

### Customer Table:

| CustomerId | FirstName | LastName | Email                        |
|------------|-----------|----------|------------------------------|
| 101        | Harry     | Potter   | harry.potter@gmail.com       |
| 102        | Ron       | Weasley  | ron.weasley@yahoo.com        |
| 103        | Hermione  | Granger  | hermione.granger@hotmail.com |
| 104        | Draco     | Malfoy   | draco.malfoy@juno.com        |

### Order Table:

| OrderId | CustomerId | OrderDate  |
|---------|------------|------------|
| 101     | 101        | 2017-01-01 |
| 102     | 102        | 2017-01-02 |
| 103     | 103        | 2017-01-03 |
| 104     | 103        | 2017-01-04 |

- Write a query to view all customers.
select * Customer Table
- Write a query to view all customers alphabetically by last name.
select * from Customer Table order by LastName ASC|DESC
- Write a query to insert a new customer into the customer table.
USE [Customer Table]
GO

INSERT INTO [dbo].[Customer Table]
           ([CustomerId]
           ,[FirstName]
           ,[LastName]
           ,[Email])
     VALUES
           (<CustomerId, int,>
           ,<FirstName, nvarchar(200),>
           ,<LastName, nvarchar(50),>
           ,<DOB, datetime,>)
GO












- Write a query to update Harry Potter's email to harry.potter@aol.com

- Write a query to inner join the customer table with the order table.

- Write a query to show which customers have not placed an order.

- Write a query to show the number of orders for each customer.
