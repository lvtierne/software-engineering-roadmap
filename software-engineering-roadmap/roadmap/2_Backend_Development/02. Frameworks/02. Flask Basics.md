# Flask Basics

Flask is a micro web framework for Python, known for its simplicity and flexibility.

## Key Concepts
- **Routes**: Map URLs to functions.
- **Templates**: Render HTML with Jinja2 templating engine.
- **Request and Response**: Handle incoming data and return responses.
- **Flask Extensions**: Add functionality to Flask applications.

## Example
```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def home():
    return "Hello, Flask!"

if __name__ == '__main__':
    app.run(debug=True)
```

## Learning Resources

- [Flask Official Documentation](https://flask.palletsprojects.com/en/3.0.x/)
- [Miguel Grinberg's Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)

## Next Steps

1. Build a small Flask application with routes and templates.
2. Explore Flask extensions for added functionality.
