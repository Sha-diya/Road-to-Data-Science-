# Day 06: Python Fundamentals - Functions

## Introduction to Functions

In Python, functions are blocks of code that can be executed when called. They provide the following advantages:
- **Code reusability**: Functions allow us to write code that can be reused multiple times.
- **Modularity**: Functions make the code modular by breaking it into smaller, manageable pieces.

### Types of Functions:
- **Built-in functions**: These are pre-defined functions in Python, like `print()`, `len()`, etc.
- **User-defined functions**: These are functions defined by the user using the `def` keyword.
- **Lambda functions**: These are anonymous functions defined using the `lambda` keyword.

## User-Defined Functions

A user-defined function is created using the `def` keyword. For example, a simple function to check if a number is even or odd is shown below:

```python
def is_even(number):
    """Check if a number is even or odd."""
    if number % 2 == 0:
        return "Even"
    else:
        return "Odd"
```
## Using __doc__ Attribute:
Every Python function has a __doc__ attribute that stores the function's documentation.You can print this documentation like this:

```python
print(is_even.__doc__)
```
## Function Parameters and Arguments
- **Parameter:** A variable in the function definition that accepts values.
- **Argument:** The actual value passed to the function when it is called.

 ### Types of Arguments:
1. **Default arguments:** These are arguments with default values.
```python
def power(a=1, b=1):
    return a ** b
```
2. **Positional arguments:** These arguments are passed in the order defined in the function.
```python
power(2, 3)
```
3. **Keyword arguments:** These arguments are passed by explicitly naming the parameters.
```python
power(b=2, a=2)
```
## Special Arguments
1. ***args:** This allows a function to accept a variable number of non-keyword arguments.
```python
def multiply(*args):
    product = 1
    for num in args:
        product *= num
    return product
```
2. ****kwargs:** This allows a function to accept a variable number of keyword arguments.
```python
def display(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")
```
## Function Execution in Memory
Python functions are executed in memory, involving:
- **Memory Layout:** Each function execution creates a stack frame in memory.
- **Garbage Collection:** Unused or unreachable objects are cleaned up by the garbage collector.

## Variable Scope
- **Global variables:** These are variables defined outside any function and can be accessed anywhere in the program.
- **Local variables:** These are variables defined within a function and can only be accessed inside that function.
  
```python
x = 10  # Global variable

def my_function():
    x = 20  # Local variable
    print(x)  # Prints the local variable

my_function()
print(x)  # Prints the global variable
```
## Nested Functions
A nested function is a function defined inside another function. The inner function can access the outer function's variables and parameters.
```python
def outer_function():
    def inner_function():
        return "Hello from inner function!"
    return inner_function()

print(outer_function())
```
## First-Class Functions
In Python, functions are first-class citizens, meaning they can:
- Be passed as arguments to other functions.
- Be returned from other functions.
- Be assigned to variables or stored in data structures.
```python
def greet(name):
    return f"Hello, {name}!"

def execute_function(func, value):
    return func(value)

print(execute_function(greet, "Alice"))
```
## Lambda Functions
Lambda functions are small, anonymous functions defined with the lambda keyword. They are often used for short, one-time operations.

Example: A lambda function to calculate the square of a number:
```python
square = lambda x: x ** 2
print(square(4))  # Output: 16
```
## Benefits of Functions
- Modularity: Functions break down complex tasks into smaller, manageable pieces.
- Readability: Functions improve code readability by naming operations clearly.
- Reusability: Functions allow code to be reused, reducing redundancy.

P## roblems Solved in the Notebook
1. **Check Odd or Even**
- Problem: Write a function is_even that checks whether a given number is odd or even.
- Solution: The program uses input from the user and prints whether the number is "Odd" or "Even".

2. **Power Calculation**
- Problem: Create a function power to calculate the power of two numbers using default, positional, and keyword arguments.

3. **Multiplication of Multiple Numbers**
- Problem: Use *args to create a function multiply that takes multiple numbers as input and returns their product.

4. **Display Key-Value Pairs**
- Problem: Use **kwargs to create a function display that accepts multiple keyword arguments and displays them in key-value format.

5. **Variable Scope Problems**
- Problem: Demonstrates the behavior of variables in different scopes (global vs local) with examples.

6. **Nested Functions**
- Problem: Demonstrates the concept of nested functions and how to return or call functions within another function.

7. **Lambda Functions**
- Problem: Write a lambda function to calculate the square of a number.

8. **Function as First-Class Citizen**
- Problem: Demonstrates function assignments, storage in data structures, and passing functions as arguments.

These practical examples reinforce the theoretical concepts explained in the notebook.
