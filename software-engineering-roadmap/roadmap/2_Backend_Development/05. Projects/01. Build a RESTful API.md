# Project: Build a RESTful API

Create a RESTful API to handle CRUD (Create, Read, Update, Delete) operations.

## Objective
- Build an API that allows users to perform CRUD operations on resources.

## Features
- **Create**: Add new resources.
- **Read**: Retrieve existing resources.
- **Update**: Modify resources.
- **Delete**: Remove resources.

## Example
```javascript
// Example Express.js RESTful API endpoints
const express = require('express');
const app = express();
app.use(express.json());

let items = []; // In-memory store

// Create
app.post('/items', (req, res) => {
    const item = req.body;
    items.push(item);
    res.status(201).json(item);
});

// Read
app.get('/items', (req, res) => {
    res.json(items);
});

// Update
app.put('/items/:id', (req, res) => {
    const id = parseInt(req.params.id);
    const updatedItem = req.body;
    items = items.map((item, index) => index === id ? updatedItem : item);
    res.json(updatedItem);
});

// Delete
app.delete('/items/:id', (req, res) => {
    const id = parseInt(req.params.id);
    items = items.filter((_, index) => index !== id);
    res.status(204).end();
});

app.listen(3000, () => {
    console.log('API running on port 3000');
});
```

## Learning Resources

- [REST API Design Tutorial](https://restfulapi.net/)
- [Building a RESTful API with Express](https://blog.postman.com/how-to-create-a-rest-api-with-node-js-and-express/)

## Next Steps

1. Deploy your API using platforms like Heroku or Vercel.
2. Implement authentication and authorization.
