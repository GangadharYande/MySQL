# SQL Query: Simplest Join

## Description
Suppose we have a `Student` table and a `batch` table with `n` and `m` columns respectively.

### Table: Students 
![Students Table](https://github.com/GangadharYande/MySQL/assets/36783781/66a8e6a3-d915-455d-bd45-1990c932d2e9)

### Table: Batches
![Batches Table](https://github.com/GangadharYande/MySQL/assets/36783781/db47e015-17c7-4ad1-96af-f83cde5b099d)

The query below illustrates a basic join operation.

## Query
```sql
SELECT * 
FROM Student 
JOIN batch;
```
### Result Table 
![image](https://github.com/GangadharYande/MySQL/assets/36783781/69e91616-c6ac-4696-b737-b042d7d16c8d)

This is the simplest Joins where it can't be handy everywhere. We need to Specify where "How To Join"
like from the above table, we can match or join two tables on certain conditions.  To make it simpler  we will use Alias in Query 's' and 'b'.


```SQL
SELECT * 
FROM Students s
JOIN batches b
ON s.batch_id = b.batch_id;
```
### Result Table 

![image](https://github.com/GangadharYande/MySQL/assets/36783781/ac2eb2a9-70f8-4687-b4fd-e3b4214c79d9)

we can use multiple table to Join
```SQL
SELECT *
FROM Students s
JOIN batches b ON s.batch_id = b.batch_id
JOIN instructor i ON b.batch_id = i.batch_id;
```
