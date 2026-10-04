# DML and DDL commands. Complex SQL expressions

## Homework Assignment Description

1. Create a database to manage a book library according to the structure shown below. Use DDL commands to create the necessary tables and their relationships.

```Структура БД
a) Назва схеми — "LibraryManagement"
b) Таблиця "authors":
author_id (INT, автоматично зростаючий PRIMARY KEY)
author_name (VARCHAR)
c) Таблиця "genres":
genre_id (INT, автоматично зростаючий PRIMARY KEY)
genre_name (VARCHAR)
d) Таблиця "books":
book_id (INT, автоматично зростаючий PRIMARY KEY)
title (VARCHAR)
publication_year (YEAR)
author_id (INT, FOREIGN KEY зв'язок з "Authors")
genre_id (INT, FOREIGN KEY зв'язок з "Genres")
e) Таблиця "users":
user_id (INT, автоматично зростаючий PRIMARY KEY)
username (VARCHAR)
email (VARCHAR)
f) Таблиця "borrowed_books":
borrow_id (INT, автоматично зростаючий PRIMARY KEY)
book_id (INT, FOREIGN KEY зв'язок з "Books")
user_id (INT, FOREIGN KEY зв'язок з "Users")
borrow_date (DATE)
return_date (DATE)
```

2. Fill in the tables with simple, made-up test data. One or two rows in each table will suffice.

3. Go to the database you worked with in Lesson 3. Write a query using the FROM and INNER JOIN operators that combines all the data tables we imported from the files: order_details, orders, customers, products, categories, employees, shippers, and suppliers. To do this, you must identify the common keys.\
   Verify that the query executes correctly.

4. Execute the queries listed below.

- Determine how many rows you received (using the COUNT statement).
- Change some of the INNER joins to LEFT or RIGHT joins. Determine what happens to the number of rows. Why? Write your answer in a text file.
- Based on the query from step 3, do the following: select only those rows where employee_id > 3 and ≤ 10.
- Group by category name, count the number of rows in each group, and calculate the average quantity of goods (the quantity of goods is stored in order_details.quantity)
- Filter out the rows where the average quantity is greater than 21.
- Sort the rows in descending order by the number of rows.
- Display (select) four rows, omitting the first row.
