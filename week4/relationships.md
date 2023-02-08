# Table relationships:

- Common relationships: 
    - one to one.
    - one to many.
    - many to many.


- Relational model:
    - it consists of 3 main concepts:
        - Data,
        - relationships,
        - constraints.

    - Some of the keywords we will face in the relational model:
        - Relation (table), Column, Row (Record or tuple).
        - Domain (The domain of the accepted data for column.)
        - Key: the unique identifier.
        - Degree: how many columns.
        - Cardinality: how many records.  
        - Constraints: key, domain and referential.

    - To define the parent, ask a question, can it exist without a child ? if yes, so it is the parent. if no, it is the child.

    - Key types:
        - PRI: primary key.
        - UNI: unique key.
        - MUL: multiple occurrences key (like foreign keys)
---
# Entities:
- Any single object in the database like a customer or an order is an entity with related attributes.
    - table is representing the entity columns are representing the entity attributes.
    - Attributes types: 
        - Simple: an attribute that can not be classified further.
        - Composite: an attribute that can be split into different components (Full name -> first and last)
        - Single Valued: like date of birth
        - Multi Valued: an attribute containing multiple values (not recommended)
        - Derived: an attribute derived from another attribute (Age from DOB)
        - Key: like primary or foreign keys.