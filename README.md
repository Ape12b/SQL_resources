# SQL Questions and Answers

1. **What is SQL?**  
   SQL (Structured Query Language) is a standard programming language designed for managing and interacting with relational databases. It is used to query, insert, update, delete, and manipulate data stored in tabular formats.

2. **What is the difference between INNER JOIN and LEFT JOIN?**  
   - **INNER JOIN**: Retrieves only the matching rows between the two tables based on the specified condition. Rows without matches are excluded.
   - **LEFT JOIN**: Retrieves all rows from the left table and the matching rows from the right table. If no match exists, the right table columns show `NULL`.

3. **What is a primary key in SQL?**  
   A primary key is a column (or combination of columns) that uniquely identifies each row in a table. It ensures uniqueness and non-nullability, and no two rows can have the same value for the primary key.

4. **What is a foreign key in SQL?**  
   A foreign key is a column (or set of columns) in one table that establishes a relationship with the primary key in another table. It ensures referential integrity by linking data between tables.

5. **Explain the different types of SQL joins.**  
   - **INNER JOIN**: Returns rows that have matching values in both tables.
   - **LEFT JOIN**: Returns all rows from the left table and matching rows from the right table. Non-matching rows in the right table are filled with `NULL`.
   - **RIGHT JOIN**: Returns all rows from the right table and matching rows from the left table. Non-matching rows in the left table are filled with `NULL`.
   - **FULL JOIN**: Combines the results of both LEFT and RIGHT JOINs, returning all rows from both tables and filling `NULL` where matches are not found.
   - **CROSS JOIN**: Produces a Cartesian product, pairing each row from one table with every row from the other table.

6. **What is normalization? Explain different normal forms.**  
   Normalization is the process of organizing data in a database to reduce redundancy and improve data integrity. The normal forms include:
   - **1NF**: Ensures that each column contains atomic values and each row is unique.
   - **2NF**: Removes partial dependencies; all non-key attributes depend on the entire primary key.
   - **3NF**: Removes transitive dependencies; non-key attributes depend only on the primary key.
   - **BCNF**: A stricter version of 3NF, ensuring that every determinant is a candidate key.
   - **4NF**: Removes multi-valued dependencies.
   - **5NF**: Addresses join dependencies.

7. **What is denormalization?**  
   Denormalization is the process of introducing redundancy into a database to improve query performance. It combines tables or adds duplicate data to reduce the need for joins.

8. **What is the difference between WHERE and HAVING?**  
   - **WHERE**: Filters rows before any aggregation is performed.
   - **HAVING**: Filters grouped or aggregated data after aggregation.

9. **What are aggregate functions in SQL?**  
   Aggregate functions perform calculations on a set of values and return a single summarizing value. Common examples include `SUM`, `COUNT`, `AVG`, `MIN`, and `MAX`.

10. **What is a subquery?**  
    A subquery is a query nested inside another query. It is used to retrieve data required for the parent query. Subqueries can return single values, multiple rows, or even a table.

11. **What is a stored procedure in SQL?**  
    A stored procedure is a predefined set of SQL statements stored in the database under a name. It can accept parameters, execute logic, and return results, similar to a function.

12. **What is a trigger in SQL?**  
    A trigger is a set of SQL statements that automatically executes when a specified event (e.g., `INSERT`, `UPDATE`, `DELETE`) occurs on a table or view. It is used to enforce business rules or maintain data integrity.

13. **What is the difference between TRUNCATE and DELETE?**  
    - **TRUNCATE**: Removes all rows from a table but keeps the table structure intact. It is faster and resets identity columns.
    - **DELETE**: Removes specific rows based on a condition and logs each deletion. It does not reset identity columns.

14. **What is a view in SQL?**  
    A view is a virtual table based on a SQL query. It does not store data itself but provides a way to encapsulate complex queries and display specific data from one or more tables.

15. **What is the ACID property in database transactions?**  
    - **Atomicity**: Ensures a transaction is all-or-nothing.
    - **Consistency**: Ensures the database remains in a valid state before and after a transaction.
    - **Isolation**: Ensures concurrent transactions do not interfere with each other.
    - **Durability**: Ensures committed transactions are permanently saved.

16. **Explain the difference between INSERT and UPDATE.**  
    - **INSERT**: Adds new rows to a table.
    - **UPDATE**: Modifies existing rows in a table based on a condition.

17. **How can you retrieve unique records from a table in SQL?**  
    Use the `DISTINCT` keyword to eliminate duplicate rows from the result set.

18. **Explain the difference between GROUP BY and ORDER BY.**  
    - **GROUP BY**: Groups rows into categories based on a key and is often used with aggregate functions.
    - **ORDER BY**: Sorts rows in ascending or descending order based on one or more columns.

19. **What is a composite key in SQL?**  
    A composite key is a combination of two or more columns that together uniquely identify a row in a table.

20. **What is a cursor in SQL?**  
    A cursor is a database object used to retrieve and manipulate query results row by row. It is useful for operations requiring iterative processing.

21. **What is a schema in SQL?**  
    A schema is a logical structure that organizes database objects such as tables, views, and indexes. It acts as a namespace for database objects.

22. **What is the difference between CHAR and VARCHAR in SQL?**  
    - **CHAR**: Fixed-length string. Always uses the defined space, padding with spaces if necessary.
    - **VARCHAR**: Variable-length string. Uses only the space required for the data, up to the maximum length defined.

23. **What are the different types of indexes in SQL?**  
    - **Clustered Index**: Rearranges the table data to match the index.
    - **Non-Clustered Index**: Creates a separate structure to store the index.
    - **Unique Index**: Ensures all values in a column are unique.
    - **Composite Index**: Index on multiple columns.
    - **Full-Text Index**: Optimized for text searching.
    - **Bitmap Index**: Efficient for low-cardinality columns.
    - **Spatial Index**: Used for geographic data.
    - **Filtered Index**: Indexes a subset of rows based on a condition.
