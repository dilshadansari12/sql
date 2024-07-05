## DataBase

`A software application used to manage our DB is called DBMS (Database Management System)
Database is collection of data in a format that can be easily accessed (Digital)`

`Three are two type od Database`

1️⃣ Relational Databases (e.g., MySQL, PostgreSQL) organize data into tables. 
 
2️⃣ NoSQL Databases (e.g., MongoDB, Cassandra) store data in formats like documents or key-value pairs. In-Memory Databases (e.g., Redis) store data in RAM for faster access.


# SQl DataBase

```javascript
SQL(Structured Query lang) is a standardized language used to manage
and manipulate relational databases. It allows users to perform
various operations on data stored in a database, such as querying,
inserting, updating, and deleting data. SQL is essential for
retrieving and managing data efficiently, and it supports functions
like sorting, filtering, and aggregating data. Common SQL commands
include SELECT, INSERT, UPDATE, DELETE, CREATE, and ALTER.
```

## SQL BASIC


`DATATYPE :-`

`Numeric Data Types`
- `INT` / `INTEGER`: Standard integer value.
- `SMALLINT`: Smaller range integer.
- `TINYINT`: Very small integer.
- `MEDIUMINT`: Medium range integer.
- `BIGINT`: Large range integer.
- `FLOAT`: Single-precision floating-point number.
- `REAL`: Single-precision floating-point, similar to `FLOAT`.
- `DOUBLE PRECISION`: Double-precision floating-point number.
- `DECIMAL`: Fixed-point number, exact precision.
- `NUMERIC`: Similar to `DECIMAL`, exact precision.

`String Data Types`
- `CHAR(n)`: Fixed-length character string.
- `VARCHAR(n)`: Variable-length character string.
- `TEXT`: Large text data.
- `TINYTEXT`: Small text data.
- `MEDIUMTEXT`: Medium-sized text data.
- `LONGTEXT`: Very large text data.
- `BINARY(n)`: Fixed-length binary data.
- `VARBINARY(n)`: Variable-length binary data.
- `BLOB`: Large binary data.
- `TINYBLOB`: Small binary data.
- `MEDIUMBLOB`: Medium-sized binary data.
- `LONGBLOB`: Very large binary data.

`Date and Time Data Types`
- `DATE`: Calendar date (YYYY-MM-DD).
- `TIME`: Time of day (HH:MM:SS).
- `DATETIME`: Date and time (YYYY-MM-DD HH:MM:SS).
- `TIMESTAMP`: Auto-updated date and time.
- `YEAR`: Year value (YYYY).

`Boolean Data Type`
- `BOOLEAN` / `BOOL`: True or false value.

`Other Data Types`

- `UUID`: Universally Unique Identifier.
- `ARRAY`: Array of values.
- `JSON`: JSON formatted data.
- `XML`: XML formatted data.
- `GEOMETRY`: Spatial data.
- `ENUM`: Enumeration type, predefined set of values.



## Functions 

`Numeric function`

### Common Numeric Functions

1. **`ABS()`**: Returns the absolute value of a number.
    ```sql
    SELECT ABS(-10); -- Result: 10
    ```

2. **`CEIL()` / `CEILING()`**: Rounds a number up to the nearest integer.
    ```sql
    SELECT CEIL(4.2); -- Result: 5
    SELECT CEILING(4.2); -- Result: 5
    ```

3. **`FLOOR()`**: Rounds a number down to the nearest integer.
    ```sql
    SELECT FLOOR(4.8); -- Result: 4
    ```

4. **`ROUND()`**: Rounds a number to a specified number of decimal places.
    ```sql
    SELECT ROUND(4.567, 2); -- Result: 4.57
    ```

5. **`POWER()`**: Raises a number to the power of another number.
    ```sql
    SELECT POWER(2, 3); -- Result: 8
    ```

6. **`SQRT()`**: Returns the square root of a number.
    ```sql
    SELECT SQRT(16); -- Result: 4
    ```

7. **`EXP()`**: Returns `e` raised to the power of a number.
    ```sql
    SELECT EXP(1); -- Result: 2.718281828459045
    ```

8. **`LN()` / `LOG()`**: Returns the natural logarithm of a number.
    ```sql
    SELECT LN(2.718281828459045); -- Result: 1
    SELECT LOG(10); -- Result: 2.302585092994046
    ```

9. **`LOG10()`**: Returns the base-10 logarithm of a number.
    ```sql
    SELECT LOG10(100); -- Result: 2
    ```

10. **`SIGN()`**: Returns the sign of a number (-1, 0, or 1).
    ```sql
    SELECT SIGN(-15); -- Result: -1
    SELECT SIGN(0);   -- Result: 0
    SELECT SIGN(25);  -- Result: 1
    ```

11. **`PI()`**: Returns the value of π.
    ```sql
    SELECT PI(); -- Result: 3.141592653589793
    ```


```sql
INSERT INTO numbers (value) VALUES (4.5), (-3.7), (0), (9.2);
```

### Aggregate Functions

1. **`SUM()`**: Calculates the total sum of values in a column.
   
2. **`AVG()`**: Computes the average of values in a column.
   
3. **`COUNT()`**: Counts the number of rows or non-null values in a column.
   
4. **`MIN()`**: Finds the minimum value in a column.
   
5. **`MAX()`**: Finds the maximum value in a column.

```sql  
SELECT SUM(mark) FROM student;  
 ```

 ### String Functions

1. **`CONCAT()`**: Concatenates two or more strings together.
   
2. **`UPPER()`**: Converts a string to uppercase.
   
3. **`LOWER()`**: Converts a string to lowercase.
   
4. **`SUBSTRING()` / `SUBSTR()`**: Extracts a substring from a string.
   
5. **`LENGTH()` / `LEN()`**: Returns the length of a string.
   
6. **`TRIM()`**: Removes leading and trailing spaces from a string.
   
7. **`LEFT()`**: Returns the leftmost characters of a string.
   
8. **`RIGHT()`**: Returns the rightmost characters of a string.
   
9. **`REPLACE()`**: Replaces occurrences of a substring within a string.
   
10. **`CHAR_LENGTH()`**: Returns the number of characters in a string.
   
11. **`POSITION()`**: Returns the position of a substring within a string.
   
12. **`CONCAT_WS()`**: Concatenates strings with a specified separator.


### Date and Time Functions

1. **`CURRENT_DATE`**: Returns the current date.
   
2. **`CURRENT_TIME`**: Returns the current time.
   
3. **`CURRENT_TIMESTAMP`**: Returns the current date and time.
   
4. **`DATE()`**: Extracts the date part from a datetime expression.
   
5. **`TIME()`**: Extracts the time part from a datetime expression.
   
6. **`EXTRACT()`**: Extracts parts (year, month, day, etc.) from a datetime.
   
7. **`DATE_ADD()` / `DATE_SUB()`**: Adds or subtracts a duration to/from a date or datetime.
   
8. **`DATEDIFF()`**: Computes the difference between two dates.
   
9. **`DATE_FORMAT()`**: Formats a date or datetime.
   
10. **`DAY()`**: Returns the day of the month from a date.
   
11. **`MONTH()`**: Returns the month from a date.
   
12. **`YEAR()`**: Returns the year from a date.


### NULL Functions

1. **`IS NULL`**: Checks if a value is NULL.
   
2. **`IS NOT NULL`**: Checks if a value is not NULL.
   
3. **`COALESCE()`**: Returns the first non-NULL value from a list of expressions.
   
4. **`NULLIF()`**: Returns NULL if two expressions are equal, otherwise returns the first expression.



### Operators in SQL

#### Arithmetic Operators

1. **`+`**: Addition.
2. **`-`**: Subtraction.
3. **`*`**: Multiplication.
4. **`/`**: Division.
5. **`%`**: Modulus (remainder).

#### Comparison Operators

1. **`=`**: Equal to.
2. **`<>` or `!=`**: Not equal to.
3. **`<`**: Less than.
4. **`>`**: Greater than.
5. **`<=`**: Less than or equal to.
6. **`>=`**: Greater than or equal to.

#### Logical Operators

1. **`AND`**: Logical AND.
2. **`OR`**: Logical OR.
3. **`NOT`**: Logical NOT.
4. **`IN`**: Checks if a value matches any value in a list.
5. **`BETWEEN`**: Checks if a value is within a range.
6. **`ALL`**: Compares a value to all values in a list.
7. **`LIKE`**: Searches for a pattern in a string.
8. **`ANY`**: Compares a value to any value in a list.

#### Bitwise Operators

1. **`&`**: Bitwise AND.
2. **`|`**: Bitwise OR.
3. **`^`**: Bitwise XOR.
4. **`~`**: Bitwise NOT.

#### Concatenation Operator

1. **`||`**: Concatenates strings (in some SQL databases).

#### NULL-related Operators

1. **`IS NULL`**: Checks if a value is NULL.
2. **`IS NOT NULL`**: Checks if a value is not NULL.


`Types of SQL Commands`

![type of sql command](https://static.wixstatic.com/media/36ae11_95f7fe4fc5654de79561a1c54bef440e~mv2.gif)