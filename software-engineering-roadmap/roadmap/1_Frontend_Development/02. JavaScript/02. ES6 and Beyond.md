# ES6 and Beyond

ECMAScript 6 (ES6) introduced many new features to JavaScript that simplify coding and improve performance.

## Key Features
- **Arrow Functions**: Shorter syntax for functions.
- **Template Literals**: Multi-line strings and string interpolation.
- **Destructuring**: Extract values from arrays and objects.
- **Modules**: Import and export code between files.
- **Promises**: Simplified handling of asynchronous operations.

## Example
```javascript
// Arrow function
const add = (a, b) => a + b;

// Template literal
const name = 'World';
console.log(`Hello, ${name}!`);

// Destructuring
const [first, second] = [1, 2];
const {x, y} = {x: 10, y: 20};

// Promises
fetch('https://api.example.com')
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error('Error:', error));
```

## Learning Resources

- [MDN Web Docs: ES6 In Depth](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules)
- [Babel: Learn ES6](https://babeljs.io/docs/learn)

## Next Steps

1. Refactor old JavaScript code using ES6 features.
2. Explore additional features like `async/await` and generators.
