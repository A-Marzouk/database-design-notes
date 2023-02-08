# CRUD Operations notes:

- INSERT INTO SELECT STATEMENT:
    - It is used to insert data to one table from another table.
    - Syntax is easy, instead of writing content,   retrieve it from another table.
    - ex: `INSERT INTO students (first_name) (SELECT name FROM departments limit 1)`

### Note that here you will not use the VALUES keyword, but directly you will type the select statement.
- Update data in a table: `UPDATE table_name SET column_name = 'value_here' WHERE condition`
    - Note that id you don't specify the condition all the data will be updated. same with delete statement.