# MongoDB Basics

MongoDB is a NoSQL database that stores data in flexible, JSON-like documents.

## Key Concepts
- **Document**: A record in MongoDB, similar to a row in SQL, stored in JSON format.
- **Collection**: A group of documents, similar to a table in SQL.
- **Database**: A collection of collections.

## Example: Basic MongoDB Commands
```javascript
// Insert a document into a collection
db.users.insertOne({ name: "John Doe", age: 25, email: "johndoe@example.com" });

// Find a document in a collection
db.users.find({ name: "John Doe" });

// Update a document in a collection
db.users.updateOne({ name: "John Doe" }, { $set: { age: 26 } });

// Delete a document from a collection
db.users.deleteOne({ name: "John Doe" });
```

## Learning Resources

- [MongoDB Basics - MongoDB University](https://university.mongodb.com/)
- [MongoDB Tutorial - W3Schools](https://www.w3schools.com/mongodb/)

## Next Steps

1. Explore MongoDB's aggregation framework.
2. Learn about indexing and querying in MongoDB.
