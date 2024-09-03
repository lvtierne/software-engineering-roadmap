# Project: Simple Blog Backend

Create a backend system for a blog with functionalities to manage posts and comments.

## Objective
- Build a backend application to manage blog posts and comments.

## Features
- **Create Post**: Add new blog posts.
- **Retrieve Posts**: List all posts.
- **Update Post**: Edit existing posts.
- **Delete Post**: Remove posts.
- **Add Comment**: Allow users to comment on posts.
- **Retrieve Comments**: List comments for a post.

## Example
```javascript
// Example Express.js server for a simple blog
const express = require('express');
const app = express();
app.use(express.json());

let posts = [];
let comments = [];

// Create Post
app.post('/posts', (req, res) => {
    const post = req.body;
    posts.push(post);
    res.status(201).json(post);
});

// Retrieve Posts
app.get('/posts', (req, res) => {
    res.json(posts);
});

// Update Post
app.put('/posts/:id', (req, res) => {
    const id = parseInt(req.params.id);
    const updatedPost = req.body;
    posts = posts.map((post, index) => index === id ? updatedPost : post);
    res.json(updatedPost);
});

// Delete Post
app.delete('/posts/:id', (req, res) => {
    const id = parseInt(req.params.id);
    posts = posts.filter((_, index) => index !== id);
    res.status(204).end();
});

// Add Comment
app.post('/posts/:id/comments', (req, res) => {
    const id = parseInt(req.params.id);
    const comment = req.body;
    comments.push({ postId: id, ...comment });
    res.status(201).json(comment);
});

// Retrieve Comments
app.get('/posts/:id/comments', (req, res) => {
    const id = parseInt(req.params.id);
    res.json(comments.filter(comment => comment.postId === id));
});

app.listen(3000, () => {
    console.log('Blog API running on port 3000');
});
```

## Learning Resources

- [Building a Blog API with Node.js](https://www.geeksforgeeks.org/how-to-build-node-js-blog-api/)
- [Full Stack Blog Tutorial](https://medium.com/@santiagobedoa/building-a-full-stack-blog-application-a-step-by-step-tutorial-ad9067a8ec90)

## Next Steps

1. Implement user authentication for posts and comments.
2. Add features like categories and tags for posts.
