# Designing databases schema:

- General meaning: It is a blueprint of how your database looks like, or an organization of information and relationships between them.

- It is different from one database to another:
    - `MySQL`: a schema is a collection of data structures (Tables) in the database and how they are stored.
    - `SQL Server`: a schema is a collection of individual components like tables, fields and keys and the relation between them.
    - ` PostgreSQL`: a namespace with named database objects(views, indexes, functions), so a schema is a namespace inside a database.
    - `Oracle`: here we assign a schema to each user.

- The concepts we care about: 
    - Organization of data in tables.
    - The relationships between them.

- Database schema consists of:
    - Data relationships.
    - Unique object keys.
    - Name and data type of columns.

- Advantages:
    - logical grouping.
    - accessibility.
    - security.
    - transfer ownerships.