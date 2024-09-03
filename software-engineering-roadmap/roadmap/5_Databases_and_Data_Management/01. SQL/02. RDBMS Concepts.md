# RDBMS Concepts

RDBMS (Relational Database Management System) is a type of database management system that stores data in tables with relationships between them.

## Key Concepts
- **Primary Key**: A unique identifier for a record in a table.
- **Foreign Key**: A field in one table that refers to the primary key in another table, establishing a relationship.
- **Normalization**: The process of organizing data to minimize redundancy.
- **ACID Properties**: 
  - **Atomicity**: Transactions are all-or-nothing.
  - **Consistency**: Data must be valid according to rules.
  - **Isolation**: Transactions occur independently.
  - **Durability**: Once a transaction is committed, it is permanent.

## Example: Table Relationships
```sql
-- Creating two related tables
CREATE TABLE departments (
    id INT PRIMARY KEY,
    department_name VARCHAR(100)
);

CREATE TABLE employees (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    department_id INT,
    FOREIGN KEY (department_id) REFERENCES departments(id)
);
```

## Learning Resources

- [RDBMS Concepts - GeeksforGeeks](https://www.geeksforgeeks.org/rdbms-full-form/)
- [ACID Properties - Tutorialspoint](https://www.tutorialspoint.com/dbms/dbms_transaction.htm)

## Next Steps

1. Understand the importance of normalization.
2. Practice creating and managing relationships between tables.
