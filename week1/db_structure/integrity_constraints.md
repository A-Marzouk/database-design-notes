# Integrity constraints

### Every table in a database should have rules or constraints to control its behavior. These are known as the integrity constraints.

### We have 3 types of constraints:
- Key constraints.
    -  The key constraint specifies that there should be a column, or columns, in a table that can be used to fetch data for any row.
    - This primary key should never be null or repeated.
- Domain constraints.
    - Refers to the rules defined for each field, for example an INT will not be able to store the home address.
- Referential constraints.
    - When we have a foreign key references another table, this key must exist in that table.