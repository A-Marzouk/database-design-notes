# SQL Arithmetic Operators:
## Operators are just words or characters to help you make activities on the DB.

- SQL arithmetic operators:
    - `+`, `-`, `*`, `/` and `%`.
    - to test: `SELECT 5 + 5;` will return 10.

    - Note that these operators can be used directly on columns: `SELECT column_one + column_two FROM table-name;` and it will return the sub of each.
    - Or in the `WHERE` clause, you can use these operators.
---
- SQL Comparison operators:
    - `>`, `<`, `>=`, `<=`, `=`, `<> or !=`.
    - `!<`: not less than. `!>`: not more than.
    - Same as arithmetic, you can use with select or where clause.
---
- SQL logical operators: they are used to combine more than a value to return TRUE or FALSE.
  
    - `ALL`: used to compare a value to ALL values in a list
        - ex: `select * from students where id > ALL (select id from departments);`
   
    - `AND`: compares between two booleans
        - ex: `select first_name from students where id = 1 AND last_name = 'doe'`
    
    - `ANY`: same as ALL, compares a value to ANY value in the list. 
        - it is used with a select statement like ALL. 
    
    - `BETWEEN`: tests an expression against a range.
        - ex: `select * from students where id BETWEEN 1 AND 3;`, not that 1 and 3 are included.
    
    - `EXISTS`: checks if the value exists in a list.
        - syntax: 
        `SELECT column_name FROM table_name WHERE [NOT] EXISTS (sub query)`
        - ex: `select * from students where EXISTS (select id from departments);` so the sub query should return at least one row for the main query to be executed.
    
    - `IN`: SELECT * FROM students WHERE id  IN (2,3)
    
    - `LIKE`: to compare column value to another value or patters. and it is applied only on char and varchar.

    - `NOT`: select * from students where id  NOT IN (2,3)
    
    - `OR`:compares between two booleans like AND.

    - `SOME`: same way of using ALL and ANY.

    - `IS NULL`: to compare if the value is NULL.
---
### Revise the [w3schools](https://www.w3schools.com/sql/sql_any_all.asp) url fro more SQL operators and functions.