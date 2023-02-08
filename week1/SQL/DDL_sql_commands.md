### DDL: The Data Definition Language provides commands for defining, deleting and modifying tables in the database.
- CREATE command:
    - create a database: `CREATE DATABASE college;`
        - to show databases: `SHOW DATABASES;`
        - to select it: `USE college;`
        - to show current database: `SELECT DATABASE();`
    - create a table with columns: `CREATE TABLE table_name (column_name1 datatype(size), column_name2 datatype(size), column_name3 datatype(size));`
        - to show tables: `SHOW TABLES;` 
        - to show all data in a table: `SELECT * FROM  table_name;`
        - to see the table structure: `DESCRIBE table_name;`

- DROP command:
    - drop a table in the db: `DROP TABLE table_name`
    - drop a database: `DROP DATABASE db_name`

- ALTER command: 
    - To change the structure of the tables such as changing the name of a table, adding a primary key to a table, or adding or deleting a column in a table.   
    - add a column in a table: `ALTER TABLE table_name ADD (column_name datatype(size))`
    - add a primary key to the table: `ALTER TABLE table_name ADD PRIMARY KEY (column_name)`
    - change a column: `ALTER TABLE table_name CHANGE old_column_name new_column_name datatype(size) options(like auto_increment and primary key)`
    - set a foreign key: 
    `ALTER TABLE table_name ADD CONSTRAINT constraint_name FOREIGN KEY (column_name_on_my_table) REFERENCES parent_table(column_name_on_referred_table)`
    - drop a column:
    `ALTER TABLE table_name DROP COLUMN column_name`
    - modify a column:
    `ALTER TABLE table_name MODIFY column_name datatype(size)`
- TRUNCATE command:
    - remove all the records from a table: `TRUNCATE TABLE table_name;`

### To comment a line in sql files use the double dash: `-- it is a comment`

### To show constraints in your database: 
`select * from information_schema.table_constraints where constraint_schema = 'db_name'`