# Express.js Basics

Express.js is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.

## Key Concepts
- **Middleware**: Functions that process requests and responses.
- **Routing**: Define routes and handle requests.
- **Templates**: Use view engines like EJS or Pug.

## Example
```javascript
const express = require('express');
const app = express();

// Middleware to parse JSON
app.use(express.json());

// Route to handle GET requests
app.get('/', (req, res) => {
    res.send('Hello, Express!');
});

// Start the server
app.listen(3000, () => {
    console.log('Server running at http://localhost:3000/');
});
```

## Learning Resources

- [Express Official Documentation](https://expressjs.com/)
- [MDN Web Docs: Express.js](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs)

## Next Steps

1. Build a RESTful API using Express.js.
2. Explore advanced features like middleware and error handling.
