# SQL Basics

SQL (Structured Query Language) is a domain-specific language used in programming and designed for managing and querying data in relational database management systems (RDBMS).

## Table of Contents
- [Key Concepts](#key-concepts)
  - [Tables](#tables)
  - [Queries](#queries)
  - [Conditions](#conditions)
- [Basic Syntax](#basic-syntax)
  - [SELECT Statement](#select-statement)
  - [WHERE Clause](#where-clause)
- [Conclusion](#conclusion)

## Key Concepts

### Tables

Tables are the basic unit of data storage in a relational database. They consist of rows and columns, where each row represents a record and each column represents a field or attribute of that record.

Example:

| ID | Name    | Age | Gender |
|----|---------|-----|--------|
| 1  | John    | 30  | Male   |
| 2  | Alice   | 25  | Female |
| 3  | Michael | 35  | Male   |

### Queries

SQL queries are used to retrieve or manipulate data in a database. There are several types of SQL queries:

- **SELECT**: Used to retrieve data from one or more tables.
- **INSERT**: Used to insert new records into a table.
- **UPDATE**: Used to modify existing records in a table.
- **DELETE**: Used to remove records from a table.

Example SELECT query:

```sql
SELECT Name, Age FROM Students WHERE Gender = 'Female';
```


## Conditions

Conditions are used to filter data based on specific criteria in SQL queries. Common conditions include:

- **EQUALS (=)**: Matches values that are equal.
- **NOT EQUALS (<>, !=)**: Matches values that are not equal.
- **LESS THAN (<)**: Matches values that are less than a specified value.
- **GREATER THAN (>)**: Matches values that are greater than a specified value.
- **AND, OR, NOT**: Logical operators used to combine conditions.

Example:

```sql
SELECT * FROM Employees WHERE Age > 30 AND Department = 'IT';
```

# Basic Syntax

## SELECT Statement

The SELECT statement is used to retrieve data from one or more tables in a database.

### Syntax:

```sql
SELECT column1, column2, ...
FROM table_name;
```
### WHERE Clause
The WHERE clause is used to filter records based on specific conditions.

Syntax:
```sql

SELECT column1, column2, ...
FROM table_name
WHERE condition;
```
Example:
```sql
SELECT * FROM Employees WHERE Department = 'HR';
```
### Conclusion
This Markdown file provides a basic overview of SQL, including key concepts, common queries, and basic syntax. SQL is a powerful language for managing and querying relational databases, and mastering its fundamentals is essential for working with data effectively.
