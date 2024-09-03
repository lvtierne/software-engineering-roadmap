# RESTful APIs

REST (Representational State Transfer) is an architectural style for designing networked applications.

## Key Concepts
- **Endpoints**: URLs where resources are accessed.
- **HTTP Methods**: Methods like GET, POST, PUT, DELETE used to interact with resources.
- **Status Codes**: Indicate the result of an API request (e.g., 200 OK, 404 Not Found).
- **JSON**: Common format for sending and receiving data.

## Example
```javascript
// Express.js example for a RESTful API endpoint
app.get('/api/users', (req, res) => {
    res.json([{ id: 1, name: 'Alice' }, { id: 2, name: 'Bob' }]);
});
```

## Learning Resources

- [REST API Tutorial](https://restfulapi.net/)
- [Postman: API Testing](https://www.postman.com/)

## Next Steps

1. Design your own RESTful API with various endpoints.
2. Test your API using tools like Postman.
