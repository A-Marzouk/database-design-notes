# Sorting and Filtering Data:

- `ORDER BY` clause:
    - ex: `select * from students ORDER BY first_name DESC;` will order the data alphabetically.
    - by default ASC (from a to z), you can use DESC keyword.
    - you can order by 2 or more columns: `select * from students ORDER BY first_name ASC, last_name DESC;` 
    - Sort is depending the data type of the column. string or numerical. 

- `SELECT DISTINCT`: it is used to return the values without any duplicates.
    - ex: `SELECT DISTINCT country FROM students`
    - if you will use multiple columns, you will generate the unique combination of the columns values. 
    - the DISTINCT keyword treats the NULL as a value.

- REVISE MYSQL AGGREGATE FUNCTIONS.