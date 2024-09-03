# Project: To-Do List App

Create a to-do list application to manage tasks and practice JavaScript.

## Objective
- Build a web app that allows users to add, edit, and remove tasks.

## Features
- **Add Task**: Input and save new tasks.
- **Edit Task**: Modify existing tasks.
- **Remove Task**: Delete tasks from the list.
- **Mark Complete**: Check off completed tasks.

## Example Structure
```html
<!DOCTYPE html>
<html>
<head>
    <title>To-Do List</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>My To-Do List</h1>
    <input type="text" id="task-input" placeholder="New task">
    <button onclick="addTask()">Add Task</button>
    <ul id="task-list"></ul>

    <script>
        function addTask() {
            // Function to add a new task
        }

        function removeTask(taskElement) {
            // Function to remove a task
        }
    </script>
</body>
</html>
```

## Learning Resources

- [JavaScript.info: Handling Events](https://javascript.info/events)
- [MDN Web Docs: Web Storage API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API)

## Next Steps

1. Implement JavaScript functions to handle adding, removing, and editing tasks.
2. Style your application using CSS to make it visually appealing.
