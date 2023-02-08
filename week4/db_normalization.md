# Database Normalization: 
- What is Database normalization ?
    - it is a process aims to minimize data duplications, avoid errors during data modifications and simplify data queries.
    - it removes the challenges you may face when you insert, update and delete data. 

- There are 3 fundamental normalization forms:
    - First Normal Form (1NF)
    - Second Normal Form (2NF)
    - Third Normal Form (3NF)
    - Fourth Normal Form (4NF)

We will learn some rules to make the database meet the criteria of these three normal forms.

- First normal form rules:
    - `Atomicity rule`: you can only have one single instance value of the column attribute in any cell of the table. so you don't store 2 names in one cell.
    - `remove repeated data`: you can not have repeated values in your rows, with foreign data. for example: students table can not have `course_name` as a column. any time you want to update course_name you will need to loop through all students.

- Second normal form rules:
    - `Avoid partial dependency relationships`: when you have a composite primary key, other non-key attributes should depend on both of the keys. not only on part of the keys. if so, you need to split the table into 2 tables to pass the 2NF.
    - `Functional dependency`: it is the dependency between non-key attributes and the primary key, it is okay to have that in your table, So you can retrieve any non-key values by the primary key.

- Third normal form rules:
    - `Transitive dependency is not allowed`: you can not have 2 non-key attributes depending on each others, when you change one attribute it will have a direct impact on another attribute, which can lead to misinformation. 
        - for example: surgery table has a doctor and a postal code, if you change the doctor it will directly impact the postal code.
        - So you need to split the tables.

- Fourth normal form rules:
    - `satisfy BCNF`: Boyce-Codd Normal Form:
        - it is an upgraded form of the 3NF.
        - Non primary key can not derive (or find) a primary key.
        - happens mostly when using composite primary key.
    - `No Multi valued dependency`:
        - when you have 2 or more independent columns depending on non-key column.
        - for example, you have student_name has course and hobby in one table.
        - this means you need to decompose the table.
        
| name | course | hobby |
| ---- | ------ | ----- |
| John | PHP  | Football  |
| john | C#   | drawing   |
| pop  | PHP  | volleyball|
| nani | C++  | dancing   | 

---
## Note that in the 2NF we handled the `Partial Dependency` and in the 3NF we handled the `Transitive Dependency` so in the 4NF we handle the `Multi Valued Dependency`