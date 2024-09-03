# Project: Basic Command Line Interface (CLI) Application

A CLI application interacts with the user through the command line. Building a simple CLI app will help you understand how to take user input, process data, and output results.

## Objective
- Create a basic CLI application that performs a simple task, such as a calculator, a to-do list, or a unit converter.

## Steps
1. **Choose a Task**: Decide what your CLI app will do (e.g., a basic calculator).
2. **Design the Workflow**: Plan how the user will interact with your app (e.g., input numbers, select an operation, see the result).
3. **Write the Code**: Implement the app in a programming language of your choice.
4. **Test the App**: Run your app multiple times with different inputs to ensure it works correctly.

## Example Code
### Python: Simple Calculator
```python
# Function to add two numbers
def add(x, y):
    return x + y

# Function to subtract the second number from the first number
def subtract(x, y):
    return x - y

# Function to multiply two numbers
def multiply(x, y):
    return x * y

# Function to divide the first number by the second number
def divide(x, y):
    # Check if the divisor is zero to avoid division by zero error
    if y == 0:
        return "Cannot divide by zero!"
    return x / y

# Function to display the calculator menu and handle user input
def calculator():
    # Print the operation options
    print("Select operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")
    
    # Get user choice of operation
    choice = input("Enter choice (1/2/3/4): ")
    
    # Get user input for the two numbers
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))
    
    # Perform the chosen operation and display the result
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

# This block ensures that the calculator function runs only if this script is executed directly
if __name__ == "__main__":
    calculator()
```

## Reflection
- What did you learn about handling user input and output in your chosen language?
- How can you improve or expand this CLI app?

## Next Steps
- Add more features to your CLI app, such as saving results to a file or adding error handling.
- Try building a different type of CLI app, like a to-do list manager.
