# Database Structure:

- Tables:
    - it is known as a relation, entity or Object.
    - `columns`: known also as fields or attributes.
        - each column has a data type.
        - data types can be different from database to another.
        - General data types:
            - String, Numeric, Date&Time and Binary. 
    - `row` known as a record or a tuple.
        - each row is uniquely identified with primary key.    
        - primary key can be a combination of more than one field. 
    - `Domain`: it is the values can be assigned to attribute, for example, only numbers can be assigned to the numerical domain field. 
        - basically it is to make sure the values of the field are well-defined including length and any other rules that define its function.
    ---
    ## a composite primary key:
    - when a table has 2 columns forming the primary key that can uniquely identify the table.
    
    - to add this composite primary key you can run this command:
    `ALTER TABLE table_name ADD PRIMARY KEY (column_1, column_2)`. Now you should have the primary key set to combination of these 2 columns.

---
- Key attributes: (column names)
    - `Candidate key attributes`: any attribute that contains a unique value in each row.
    - `Composite key attribute`: a key composed of 2 or more columns to form the unique identifier.
    - `Primary key`: a unique identifier like the ID.
    - `Alternate key`: a candidate key that is not selected as a primary key.
    - `Foreign Key`: an attitude that references a unique key a another table. 
