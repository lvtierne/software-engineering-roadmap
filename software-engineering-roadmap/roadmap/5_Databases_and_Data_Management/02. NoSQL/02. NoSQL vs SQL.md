# NoSQL vs. SQL

SQL and NoSQL databases serve different purposes and are designed to solve different types of problems.

## Key Differences
- **Data Model**: 
  - SQL: Structured, table-based.
  - NoSQL: Flexible, document-based, key-value pairs, column stores, or graph-based.
- **Schema**:
  - SQL: Fixed schema.
  - NoSQL: Dynamic schema.
- **Scalability**:
  - SQL: Vertical scalability.
  - NoSQL: Horizontal scalability.
- **Use Cases**:
  - SQL: Suited for complex queries, transactions, and relationships.
  - NoSQL: Suited for large volumes of unstructured or semi-structured data, and real-time applications.

## Example: SQL vs. NoSQL
```sql
-- SQL: Structured Data (Employee Record)
CREATE TABLE employees (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    department VARCHAR(100)
);

-- NoSQL: Document Store (Employee Record)
{
    "id": 1,
    "name": "John Doe",
    "age": 25,
    "department": "Sales"
}
```

## Learning Resources

- [SQL vs NoSQL - MongoDB](https://www.mongodb.com/nosql-explained)
- [SQL vs NoSQL - GeeksforGeeks](https://www.geeksforgeeks.org/difference-between-sql-and-nosql/)

## Next Steps

1. Identify scenarios where NoSQL is more appropriate than SQL, and vice versa.
2. Experiment with both types of databases on sample projects.
