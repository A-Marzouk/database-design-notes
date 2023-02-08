# Data types in MySQL Database:

### We agreed that data types can be different from one database to another.
### Generally we have 4 types of data:
- String
    - CHAR(FIXED), VARCHAR, TEXT, ENUM, SET.
- Numeric
    - TINYINT, INT, BIGINT, FLOAT, BOOL OR BOOLEAN.
- Date&Time
    - DATE, TIME, DATETIME.
- Binary: to store binary data like images.
    - BINARY, which is like CHAR (FIXED SIZE)
    - VARBINARY, like VARCHAR with variable size.
- Miscellaneous (different) data types:
    - CLOB (Character Large Object ) exists only in oracle, in MySQL we use text instead.
        - it has a very large capacity, used to store images, etc.
        - it has character encoding.
    - BLOB (Binary Large Object)
        - for storing a collection of binary data such as images.

### Note that in MySQL, TEXT and BLOB can hold maximum up to 64k (2^16 = 65536 chars). to use bigger than that you cna use the LONGTEXT and LONGBLOB.