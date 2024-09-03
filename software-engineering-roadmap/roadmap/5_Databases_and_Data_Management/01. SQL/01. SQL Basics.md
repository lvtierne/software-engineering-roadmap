# SQL Basics

SQL (Structured Query Language) is a standard language for managing and manipulating relational databases.

## Key Concepts
- **Database**: A structured set of data held in a computer.
- **Table**: A collection of related data entries consisting of rows and columns.
- **SQL Commands**: 
  - **DDL (Data Definition Language)**: `CREATE`, `ALTER`, `DROP`
  - **DML (Data Manipulation Language)**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`

## Example: Basic SQL Queries
```sql
-- Create a table
CREATE TABLE students (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    age INT
);

-- Insert data into the table
INSERT INTO students (id, name, age) VALUES (1, 'John Doe', 20);

-- Select data from the table
SELECT * FROM students;

-- Update data in the table
UPDATE students SET age = 21 WHERE id = 1;

-- Delete data from the table
DELETE FROM students WHERE id = 1;
```

## Learning Resources

- [SQL Basics - W3Schools](https://www.w3schools.com/sql/)
- [SQL Tutorial - SQLZoo](https://sqlzoo.net/)

## Next Steps

1. Practice writing basic SQL queries.
2. Explore more advanced SQL commands.
