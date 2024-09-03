# Stacks and Queues

Stacks and queues are abstract data types that serve as containers for data.

## Stacks
- **Definition**: LIFO (Last In, First Out) structure.
- **Operations**: Push (add), pop (remove), peek (view top element).

### Example: Python Stack Implementation
```python
class Stack:
    def __init__(self):
        self.stack = []

    def push(self, item):
        self.stack.append(item)

    def pop(self):
        if not self.is_empty():
            return self.stack.pop()
        raise IndexError("Pop from an empty stack")

    def peek(self):
        if not self.is_empty():
            return self.stack[-1]
        raise IndexError("Peek from an empty stack")

    def is_empty(self):
        return len(self.stack) == 0
```

## Queues
- Definition: FIFO (First In, First Out) structure.
- Operations: Enqueue (add), dequeue (remove), front (view front element).

### Example: Python Queue Implementation
```python
from collections import deque

class Queue:
    def __init__(self):
        self.queue = deque()

    def enqueue(self, item):
        self.queue.append(item)

    def dequeue(self):
        if not self.is_empty():
            return self.queue.popleft()
        raise IndexError("Dequeue from an empty queue")

    def front(self):
        if not self.is_empty():
            return self.queue[0]
        raise IndexError("Front from an empty queue")

    def is_empty(self):
        return len(self.queue) == 0
```

## Learning Resources

- [Stacks and Queues - GeeksforGeeks](https://www.geeksforgeeks.org/stack-data-structure/)
- [Stacks and Queues in Python - Tutorialspoint](https://www.tutorialspoint.com/stack-and-queue-in-python-using-queue-module#:~:text=In%20Python%2C%20it%20is%20very,the%20code%20shorter%20and%20simple.)

## Next Steps

1. Solve problems involving stacks and queues.
2. Implement additional operations and variations.
