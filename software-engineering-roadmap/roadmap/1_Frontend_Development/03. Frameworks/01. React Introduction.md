# Introduction to React

React is a JavaScript library for building user interfaces by creating reusable UI components.

## Key Concepts
- **Components**: Building blocks of React applications. They can be functional or class-based.
- **JSX**: Syntax extension that allows you to write HTML elements in JavaScript.
- **Props**: Short for properties, used to pass data to components.
- **State**: Data that changes over time and affects rendering.

## Example
```javascript
import React from 'react';
import ReactDOM from 'react-dom';

// Functional component
const App = () => {
    return <h1>Hello, React!</h1>;
};

// Render component
ReactDOM.render(<App />, document.getElementById('root'));
```

## Learning Resources

- [React Official Documentation](https://react.dev/)
- [Codecademy: Learn React](https://www.codecademy.com/learn/react-101)

## Next Steps

1. Build a simple React application.
2. Learn about React Hooks and state management.
