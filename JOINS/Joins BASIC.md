# Joins in Databases

## Overview

Joins are a fundamental concept in relational databases that allow you to combine data from two or more tables based on a related column between them. They are essential for querying data across multiple tables efficiently.

This README provides an overview of different types of joins commonly used in databases and their syntax.

## Types of Joins

### 1. INNER JOIN

An INNER JOIN returns rows that have matching values in both tables being joined.

#### Syntax:

```sql
SELECT columns
FROM table1
INNER JOIN table2
ON table1.column = table2.column;
```

### 2. LEFT JOIN (or LEFT OUTER JOIN)

A LEFT JOIN returns all rows from the left table and the matched rows from the right table. If there's no match, NULL values are returned for the right table columns.

#### Syntax:

```sql
SELECT columns
FROM table1
LEFT JOIN table2
ON table1.column = table2.column;
```

### 3. RIGHT JOIN (or RIGHT OUTER JOIN)

A RIGHT JOIN returns all rows from the right table and the matched rows from the left table. If there's no match, NULL values are returned for the left table columns.

#### Syntax:

```sql
SELECT columns
FROM table1
RIGHT JOIN table2
ON table1.column = table2.column;
```

### 4. FULL JOIN (or FULL OUTER JOIN)

A FULL JOIN returns all rows when there's a match in either left or right table. If there's no match, NULL values are returned for the columns of the table without a matching row.

#### Syntax:

```sql
SELECT columns
FROM table1
FULL JOIN table2
ON table1.column = table2.column;
```

## Conclusion

Understanding how to use joins is crucial for querying data from multiple tables in a relational database. Each type of join serves a specific purpose and knowing when to use them is essential for writing efficient and effective SQL queries.

For more information, consult the documentation of your database management system (DBMS) for specific details and examples.
