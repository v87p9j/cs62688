java c
Department of Accounting and Business Analytics
BTM 211
Management Information Systems
DB Assignment – Fall 2024
Case Study: Joshua Tree Instruments
Background
Joshua Tree Instruments (JTI) has been the top choice for musical instruments rentals in Alberta since 1987. What started as a hobby for Brian Edge, an avid guitar collector and rock enthusiast, slowly turned into a business. Now, Brian has expanded and carries the top brands in musical instruments.
After opening his first retail location in south Edmonton, Brain opened six more stores, another in northern Edmonton, two in Calgary, one in Grande Prairie, one in Red Deer, and his most recent expansion, a store in Lethbridge. With 90 employees spread out across his locations, JTI has been able to serve the Albertan community with pride and hopes to one day expand into other provinces on the Western coast while maintaining their reputation of carrying the biggest brands in instruments and the highest quality of rentals.
Problem
Brian Edge is looking to implement a database for JTI so he can manage data more effectively across his company. The database will be used not only by him but also by employees across the company at various different levels.
Using the data model provided, create a database for JTI in SQLite.
Requirements:
Part A (15 marks):
Create the SQLite database tables.
Build an SQLite database of TABLES that match the official “Joshua_Tree_Instruments_Data_Model.pdf” provided in the Assignments folder on eClass.
IMPORTANT: Do NOT use your personal data model that you built in the Data Model Assignment
1. Create each table with the correct name. You should create nine (9) tables.
2. Create all attributes for each table with the correct name and SQLite data types.
3. Implement the primary keys (or composite keys)
4. Implement each relationship for every foreign key.
Part B (15 marks):
Import data into the SQLite database.
Using the techniques you learned in the lab videos, import the provided sample data (JoshuaTreeInstruments_Data_2024_Fall.xlsx) into each table.
1. Prepare a CSV (Comma Delimited) file for each table you intend to import into your SQLite database. Name each CSV file the name of the table. You should have nine (9) CSV files in total.
Note: You will need to reformat and “clean up” the sample data spreadsheet by cutting and re-pasting some of the columns from each table into its own CSV file.
2. Using SQLite Studios "Tools - Import" function, populate your database tables with the appropriate CSV files. 
Hint: First import the “Parent” tables that act as “1” tables in 1-M relationships – then import the “Child” tables. In general, work from the outside-in on the data model.
Part C (20 marks):
Insert new data rows into tables.
Using the techniques you learned in the Labs, insert new data rows into tables
1. Create two (2) new Customers in the Customer table. Use the following information for the new customers.AttributeNew customer #1New customer #2
CustomerId
20240301
20240103
CreditCardNumber
1234567891234567
7654321987654321
RepEmpId
114
106
FamilyName
Your family name
Your Given names
GivenNames
Your Given name
You family name
EmailAddress
YourCCID@ualberta.ca (e.g. gaga1@ualberta.ca)

YourCCIDspelledbackwards @ualberta.ca (e.g. 1agag@ualberta.ca)
Address1
2587 Willow Creek Road
4391 Sunset Boulevard
Address2
Apt. 305
Suite B-12
Municipality
Brookhaven Village
Brookhaven Village
ProvinceState
Alberta
Alberta
PostalCode
T3X 4P9
T5Z 2N4
PhoneNumber
7801234567
7807654321
2. Create two (2) new rental agreements in the RentalAgreement table for each new customer created above, as well as the corresponding RentalItem(s). Use the following information for the new rental agreements and rental items:
New Rental for Customer 1:
New Rental for Customer 2:
Part D (50 marks):
Query the data in the SQLite database using Select.
Using the techniques you learned in the Labs, write a SELECT QUERY to answer the following questions based on the data in your SQLite database.
IMPORTANT: You MUST include your “working” SQL statements in this document. The code should not include any line numbers. We will copy these SQL code and test run with your database. Failure to submit working SQL will result in deductions.
Query 1 (5 marks):
Brian wants to pull a list of ever代 写BTM 211  Management Information Systems Fall 2024SQL
代做程序编程语言y rental id from his database. Write a query to display the following information (from left to right):
● RentalID
● StoreID
Important:. Do not include the line numbers when you copy and paste in the yellow box.
Copy and paste your working SQL statement in the box below:
Query 2 (5 marks):
Brian wants to see every row and column from the customer table. Write a query to display the following information (from left to right):
● CustomerId
● RepEmployeeID
● CreditCardNumber
● LastName
● GivenNames
● EmailAddress
● Address1
● Address2
● Municipality
● ProvinceState
● Country
● PostalCode
● PhoneNumber
Important:. Do not include the line numbers in the yellow box.
Copy and paste your working SQL statement in the box below:
Query 3 (5 marks):
This time, Brian wants a list of every customer, but he only wants to include their ID, name, and location. However, Brian wants the given names and last names to be in one column, and the locations in one column.
Write a query to display the following information (from left to right). Concatenate the customer names and locations and rename them with the alias name provided in quotation marks:
● CustomerID
● GivenNames and LastName as “Customer Name” (seperate each name with a space)
● Address1, Address2, Municipality, ProvinceState, and Country as “Customer Location” (seperate each name with a comma)
Important: Do not include the line numbers in the yellow box.
Copy and paste your working SQL statement in the box below:
Query 4 (5 marks):
Brian wants a list of the instrument id’s, instrument type codes, and conditions, and he wants them to be ordered by condition in ascending order. Write a query to display the following information (from left to right):
● InstrumentID
● InstrumentTypeCode
● Condition
Important: Do not include the line numbers in the yellow box.
Copy and paste your working SQL statement in the box below:
Query 5 (5 marks):
Brian wants a list of every instrument, but only if that instrument has a repair id associated with it. Write a query to display the following information (from left to right):
● InstrumentID
● InstrumentTypeCode
● RepairID
Important: Do not include the line numbers in the yellow box.
Copy and paste your working SQL statement in the box below:
Query 6 (5 marks):
Brian wants a list of every instrument that has been rented and he wants to know the total revenue received from that instrument rental. However, he only wants to see the total revenue of instruments that have an Added Warranty applied. Write a query to display the following information (from left to right):
● InstrumentID
● RentalPrice
● AddedWarranty
● A new column called “Total Revenue”
Important: Do not include the line numbers in the yellow box.
Copy and paste your working SQL statement in the box below:
Query 7 (5 marks):
Brian wants a count of the number of instruments he has in his database grouped by their instrument type code. Write a query to display the following information (from left to right):
● InstrumentTypeCode
● A new column called “Number of Instruments”
Important: Do not include the line numbers in the yellow box.
Copy and paste your working SQL statement in the box below
Query 8 (5 marks):
Brian wants a list of every instrument id, wholesale price, and rental price. He also wants it to be ordered from highest rental price to lowest. Write a query to display the following information (from left to right):
● InstrumentId
● WholesalePrice
● Rental Price
Important: Do not include the line numbers in the yellow box.
Copy and paste your working SQL statement in the box below:
Query 9 (10 marks):
Bells and Whistle Query
Brian wants you to create your own query that includes functions previously used in the assignment and at least one (1) additional “bell and whistle” function (e.g. arithmetic, scalar, math, date/time). You can use any of the tables in the database in your query.
Make sure that your query runs, as you will be deducted marks for queries that do not produce data or rows.
List the tables you used below, and the left to right order of your column names using bullet points.
Tables used:
● 
Columns used:
● 
Important: Do not include the line numbers in the yellow box.
Copy and paste your working SQL statement in the box below:



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
