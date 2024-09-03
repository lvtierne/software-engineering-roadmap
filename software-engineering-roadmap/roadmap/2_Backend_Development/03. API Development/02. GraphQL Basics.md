# GraphQL Basics

GraphQL is a query language for APIs and a server-side runtime for executing those queries.

## Key Concepts
- **Queries**: Request specific data from the server.
- **Mutations**: Modify data on the server.
- **Schemas**: Define the structure of data and operations.
- **Resolvers**: Functions that resolve queries and mutations.

## Example
```javascript
// Example schema definition in GraphQL
const { GraphQLObjectType, GraphQLSchema, GraphQLString } = require('graphql');

const RootQuery = new GraphQLObjectType({
    name: 'RootQueryType',
    fields: {
        hello: {
            type: GraphQLString,
            resolve() {
                return 'Hello, GraphQL!';
            }
        }
    }
});

module.exports = new GraphQLSchema({
    query: RootQuery
});
```

## Learning Resources

- [GraphQL Official Documentation](https://graphql.org/learn/)
- [How to GraphQL](https://www.howtographql.com/)

## Next Steps

1. Build a simple GraphQL server and client.
2. Explore advanced GraphQL features like subscriptions and authentication.
