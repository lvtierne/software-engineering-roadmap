# Basic Calculator

## Objective
Build a basic calculator application that can perform fundamental arithmetic operations: addition, subtraction, multiplication, and division.

## Features
- Input two numbers.
- Choose an operation (add, subtract, multiply, divide).
- Display the result.

## Steps
1. **Choose a Language**: Implement the calculator in a language of your choice (e.g., Python, JavaScript).
2. **Design the Interface**: Create a simple user interface (CLI or GUI) for entering numbers and selecting operations.
3. **Implement Functions**: Write functions for each arithmetic operation.
4. **Handle Errors**: Implement error handling for invalid inputs and division by zero.

## Example Code
### Python: Basic Calculator
```python
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Cannot divide by zero!"
    return x / y

def calculator():
    print("Select operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")
    
    choice = input("Enter choice(1/2/3/4): ")
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))
    
    if choice == '1':
        print(f"The result is: {add(num1, num2)}")
    elif choice == '2':
        print(f"The result is: {subtract(num1, num2)}")
    elif choice == '3':
        print(f"The result is: {multiply(num1, num2)}")
    elif choice == '4':
        print(f"The result is: {divide(num1, num2)}")
    else:
        print("Invalid Input")

if __name__ == "__main__":
    calculator()
```

## Learning Resources

- [Basic Calculator Tutorial - YouTube](https://www.youtube.com/watch?v=E8D35UOcz9Q)
