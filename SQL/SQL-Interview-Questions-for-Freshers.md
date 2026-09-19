# 🗄️ SQL Interview Questions for Freshers

A beginner-friendly collection of SQL concepts, commands, and interview questions for students preparing for placements.

---

## 📌 What is SQL?

SQL (Structured Query Language) is used to store, retrieve, manipulate, and manage data in relational databases.

Popular SQL databases include MySQL, PostgreSQL, Oracle, and SQL Server.

---

## 🔹 Basic SQL Commands

### SELECT

Used to retrieve data from a table.

    SELECT * FROM students;

### WHERE

Used to filter records.

    SELECT * FROM students
    WHERE age > 20;

### ORDER BY

Used to sort results.

    SELECT * FROM students
    ORDER BY age DESC;

### DISTINCT

Used to return unique values.

    SELECT DISTINCT city
    FROM students;

### LIMIT

Used to restrict the number of results.

    SELECT * FROM students
    LIMIT 5;

---

# 🧮 Aggregate Functions

Aggregate functions perform calculations on multiple rows.

| Function | Purpose |
|---|---|
| `COUNT()` | Counts rows |
| `SUM()` | Calculates total |
| `AVG()` | Calculates average |
| `MAX()` | Finds maximum value |
| `MIN()` | Finds minimum value |

Examples:

    SELECT COUNT(*) FROM students;

    SELECT AVG(age) FROM students;

    SELECT MAX(age) FROM students;

---

# 📊 GROUP BY

Used to group rows with the same values.

Example:

    SELECT department, COUNT(*)
    FROM students
    GROUP BY department;

---

# 🔎 HAVING

Used to filter grouped results.

Example:

    SELECT department, COUNT(*)
    FROM students
    GROUP BY department
    HAVING COUNT(*) > 5;

### WHERE vs HAVING

- `WHERE` filters rows before grouping.
- `HAVING` filters groups after `GROUP BY`.

---

# 🔗 SQL JOINS

Joins are used to combine data from multiple tables.

### INNER JOIN

Returns matching records from both tables.

    SELECT students.name, departments.department_name
    FROM students
    INNER JOIN departments
    ON students.department_id = departments.id;

### LEFT JOIN

Returns all records from the left table and matching records from the right table.

### RIGHT JOIN

Returns all records from the right table and matching records from the left table.

### FULL OUTER JOIN

Returns matching and non-matching records from both tables.

> Note: MySQL does not directly support `FULL OUTER JOIN`. It can be achieved using `LEFT JOIN`, `RIGHT JOIN`, and `UNION`.

---

# 🗝️ Keys in SQL

### Primary Key

- Uniquely identifies each row.
- Cannot contain `NULL`.
- A table has one primary key constraint, which can contain one or multiple columns.

### Foreign Key

- Creates a relationship between tables.
- Refers to a primary key or unique key in another table.

### Candidate Key

A column or combination of columns that can uniquely identify a row.

---

# 🧱 Constraints

Common SQL constraints:

- `PRIMARY KEY`
- `FOREIGN KEY`
- `NOT NULL`
- `UNIQUE`
- `DEFAULT`
- `CHECK`

Example:

    CREATE TABLE students (
        id INT PRIMARY KEY,
        name VARCHAR(50) NOT NULL,
        email VARCHAR(100) UNIQUE,
        age INT CHECK (age >= 18)
    );

---

# 🛠️ INSERT, UPDATE & DELETE

### INSERT

Adds new records.

    INSERT INTO students (id, name, age)
    VALUES (1, 'Rahul', 21);

### UPDATE

Modifies existing records.

    UPDATE students
    SET age = 22
    WHERE id = 1;

### DELETE

Removes records.

    DELETE FROM students
    WHERE id = 1;

⚠️ Always use a suitable `WHERE` condition with `UPDATE` and `DELETE` when you only want to affect specific rows.

---

# 📚 Common SQL Interview Questions

### 1. What is SQL?

SQL is a language used to interact with and manage data in relational databases.

### 2. What is a database?

A database is an organized collection of data that can be stored, accessed, and managed efficiently.

### 3. What is a primary key?

A primary key uniquely identifies each row in a table and cannot contain `NULL`.

### 4. What is a foreign key?

A foreign key is used to establish a relationship between tables by referencing a key in another table.

### 5. What is the difference between WHERE and HAVING?

`WHERE` filters individual rows, while `HAVING` filters grouped results.

### 6. What is a JOIN?

A JOIN combines related data from two or more tables.

### 7. What is the difference between DELETE, DROP and TRUNCATE?

- `DELETE` removes selected rows and can use `WHERE`.
- `TRUNCATE` removes all rows from a table.
- `DROP` removes the table itself, including its structure.

### 8. What is NULL?

`NULL` represents a missing, unknown, or unavailable value. It is not the same as `0` or an empty string.

### 9. What is normalization?

Normalization is the process of organizing database tables to reduce data redundancy and improve data integrity.

### 10. What is an index?

An index is a database structure that can improve the speed of data retrieval, with additional storage and write overhead.

---

# 🎯 Practice Questions

Try solving these yourself:

1. Find all students whose age is greater than 20.
2. Find the maximum salary from an employee table.
3. Find the average salary of employees.
4. Count the number of employees in each department.
5. Find departments having more than 5 employees.
6. Display unique cities from a student table.
7. Sort employees by salary from highest to lowest.
8. Find employees whose names start with `A`.
9. Find the second highest salary.
10. Find employees who do not belong to any department.
11. Write a query using INNER JOIN.
12. Write a query using LEFT JOIN.
13. Find duplicate values in a column.
14. Find the total salary paid by each department.
15. Find the highest salary in each department.

---

# ⚡ Quick Revision

| Concept | Purpose |
|---|---|
| `SELECT` | Retrieve data |
| `WHERE` | Filter rows |
| `DISTINCT` | Remove duplicate results |
| `ORDER BY` | Sort results |
| `GROUP BY` | Group rows |
| `HAVING` | Filter groups |
| `JOIN` | Combine tables |
| `COUNT()` | Count rows |
| `SUM()` | Find total |
| `AVG()` | Find average |
| `MAX()` | Find maximum |
| `MIN()` | Find minimum |
| `INSERT` | Add data |
| `UPDATE` | Modify data |
| `DELETE` | Remove rows |

---

