# Day 07: Python Fundamentals - Object-Oriented Programming (OOP)

## Introduction to OOP

Object-Oriented Programming (OOP) is a programming paradigm that focuses on objects and their interactions. It provides the following advantages:
- **Modularity**: Code is organized into reusable, self-contained objects.
- **Encapsulation**: Hides the internal state and exposes only the necessary parts of an object.
- **Reusability**: Enables code reuse through inheritance and polymorphism.

### Key Concepts of OOP:
- **Class**: A blueprint for creating objects.
- **Object**: An instance of a class.
- **Polymorphism**: Allows objects to be treated as instances of their parent class.
- **Encapsulation**: Hides internal details and protects object integrity.
- **Inheritance**: Enables new classes to inherit attributes and methods from existing classes.
- **Abstraction**: Focuses on essential qualities rather than specific characteristics.

---

## Classes and Objects

### Class
A class is defined using the `class` keyword. It serves as a blueprint that specifies the attributes and behaviors of an object.

```python
class ATM:
    def __init__(self):
        self.balance = 0

my_atm = ATM()  # Create an object of the ATM class
```
### Object
An object is an instance of a class. It is created using the class name and can access the attributes and methods defined in the class.

```python
print(my_atm.balance)  # Access the balance attribute
```

## Methods in Classes
### Methods in Classes
- **Methods**:  Functions defined inside a class that operate on objects.
- **Functions**: Standalone blocks of code outside any class.

```python
class ATM:
    def display_balance(self):
        print("Balance is:", self.balance)
```
### Constructor (__init__)
The notebook demonstrates an ATM simulation using OOP concepts. The ATM class includes:

## Example: ATM Class
The notebook demonstrates an ATM simulation using OOP concepts. The ATM class includes:

- **Attributes**: `pin` and `balance`.
- **Methods**:  
  --`create_pin`: Sets a new pin and balance.  
  -- `change_pin`: Updates the pin.  
  -- `check_balance`: Displays the balance.  
  -- `withdraw`: Deducts an amount from the balance if sufficient funds are available.  

```python
class ATM:
    def __init__(self):
        self.pin = ''
        self.balance = 0

    def create_pin(self):
        self.pin = input("Enter your pin: ")
        self.balance = float(input("Enter your balance: "))
```

## Key OOP Features in Practice
### Polymorphism
Illustrated using a Fraction class that overloads operators like addition (`+`) and subtraction (`-`).

```python
class Fraction:
    def __init__(self, numerator, denominator):
        self.num = numerator
        self.den = denominator

    def __add__(self, other):
        return Fraction(
            self.num * other.den + self.den * other.num,
            self.den * other.den
        )
```
### Encapsulation
Demonstrated using private attributes and getter/setter methods.

```python
class ATM:
    def __init__(self):
        self.__balance = 0

    def get_balance(self):
        return self.__balance

    def set_balance(self, new_balance):
        self.__balance = new_balance
```

### Exercises and Applications  
1. **Fraction Class**:  
   - Demonstrates operator overloading for addition, subtraction, multiplication, and division.

2. **2D Coordinates and Lines**:
   - Classes to represent points and lines in 2D space.
   - Methods to calculate distances and check if a point lies on a line.

3. **ATM Simulation**:
   - Implements a menu-driven interface for managing an ATM.

4. **Dynamic Attributes**:
   - Shows how to add attributes dynamically to an object.


### Additional Topics Covered
- **Magic Methods** (`__init__`, `__str__`): Enable customization of object behavior.
- **Nested Classes and Functions**: Functions within classes and the concept of inner functions.
- **Passing Objects as Arguments**: Demonstrates how objects can bepassed between functions.

### Problems Solved in the Notebook
1. **ATM Class Implementation**
   - Problem: Create a class for ATM functionality.
   - Solution: Includes methods for creating pins, changing pins, checking balances, and withdrawals.

2. **Fraction Operations**
   - Problem: Implement a Fraction class to handle arithmetic operations
   - Solution: Uses operator overloading for addition, subtraction, multiplication, and division.

3. **2D Geometry**
   - Problem: Create classes to handle points and lines in 2D space
   - Solution: Methods for calculating distances and verifying point-line relationships.

4. **Encapsulation**
   - Problem: Demonstrate private variables and getter/setter methods.
   - Solution: Implements encapsulation techniques in the ATM class.

5. **Dynamic Attributes**
   - Problem: Add and access attributes dynamically.
   - Solution: Demonstrated with a Person class.
     
This notebook serves as a comprehensive introduction to OOP principles with practical examples and exercises.
