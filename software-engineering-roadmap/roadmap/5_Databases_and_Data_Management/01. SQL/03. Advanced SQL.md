# Advanced SQL

Once you are comfortable with basic SQL, it's time to explore more advanced topics that allow for complex data manipulation.

## Key Topics
- **Joins**: Combining data from multiple tables (`INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, `FULL JOIN`).
- **Subqueries**: SQL queries nested inside another query.
- **Indexes**: Speeding up database queries by creating indexes.
- **Transactions**: Ensuring data integrity with `BEGIN`, `COMMIT`, and `ROLLBACK`.
- **Stored Procedures**: Reusable SQL code blocks that can be executed as a single unit.

## Example: Using Joins and Subqueries
```sql
-- Join example
SELECT employees.name, departments.department_name
FROM employees
INNER JOIN departments ON employees.department_id = departments.id;

-- Subquery example
SELECT name FROM employees WHERE department_id = (
    SELECT id FROM departments WHERE department_name = 'Sales'
);
```

## Learning Resources

- [Advanced SQL - Mode Analytics](https://mode.com/sql-tutorial/intro-to-advanced-sql)
- [SQL Joins - W3Schools](https://www.w3schools.com/sql/sql_join.asp)

## Next Steps

1. Practice writing queries with joins and subqueries.
2. Explore using indexes and transactions in your SQL queries.
