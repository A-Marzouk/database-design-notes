# SQL: structured query language.

### It is a standard language that can interact with different databases which have structured data.
### These like:
- MySQL, PostgreSQL, Oracle, Microsoft SQL Server 
### How the database is reading these instructions from SQL ?
- This is done by the use of the DMS (Database Management System) which takes the SQL and change it to a language understood by the database.
---
## SQL Subsets:
- `DDL`: Data Definition Language.
    - Used to define storage objects in your database, like creating tables.
    - Its CRUD operations are done on DB structure, not on the Data.
        - DDL Create is to create tables.
        - DDL Alter is to update tables with new column or column name.
        - DDL Drop: is to drop a table.
- `DML`: Data Manipulation Language.
    - Used to manipulate data in the database.
    - The default C`R`UD operations we know.
- `DQL`: Data Query Language.
    - To read or retrieve data using the `SELECT` command.
- `DCL`: Data Control Language. 
    - Used to control access to the database.
        - Grand And Revoke commands are used to give access privileges to users or revoke then.
---
## SQL Advantages:
- It is a standard language, compatible with all available relational databases. 
- Run on any hardware running any OS, so it is portable.
- Covers all areas of database management and administration.