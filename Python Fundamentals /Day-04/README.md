# Day_04: Python Fundamentals and Problem-Solving

This repository contains a collection of Python exercises and solutions aimed at reinforcing fundamental programming concepts. The code examples are organized into several key areas for easy reference and learning.

---

## 1. **Introduction to Lists:**
This section provides an overview of Python lists, their characteristics, and how to create, access, and manipulate them. Lists are mutable and can hold various data types.

- **Creating Lists:**
  - Lists can be created using square brackets `[]`.
  - Example: `my_list = [1, 2, 3, 4, 5]`.

- **Accessing List Elements:**
  - Use indexing and slicing to access and modify elements.
  - Example: `my_list[0]` returns `1`.

---

## 2. **Creating Lists using Type Conversion:**
This section demonstrates how to convert other data types into lists.

- **Converting a String to a List:**
  - Example: `list_from_string = list("hello")` results in `['h', 'e', 'l', 'l', 'o']`.

---

## 3. **Accessing and Editing Lists:**
Learn how to access, slice, and modify elements of a list. This section also covers methods to add, edit, and remove elements.

- **Adding Elements:**
  - `append()`, `insert()`, `extend()`.
  - Example: `my_list.append(6)`.

- **Modifying Elements:**
  - Indexing and slicing for modification.
  - Example: `my_list[0] = 10`.

- **Removing Elements:**
  - Use `remove()`, `pop()`, `del`, and `clear()`.
  - Example: `my_list.remove(6)`.

---

## 4. **Operations on Lists:**
This section introduces various operations that can be performed on lists.

- **Arithmetic Operations:**
  - Concatenate lists using `+` and repeat with `*`.
  - Example: `[1, 2] + [3, 4]` results in `[1, 2, 3, 4]`.

- **Membership Check:**
  - Check if an element exists in a list using `in`.
  - Example: `3 in my_list` returns `True`.

- **Loops and Iterations:**
  - Loop through lists using `for`.
  - Example: `for item in my_list: print(item)`.

---

## 5. **List Functions:**
This section explains built-in functions that can be used to manipulate lists.

- **Functions:**
  - `len()`, `min()`, `max()`, `sorted()`, `count()`, `index()`, etc.
  - Example: `len(my_list)` gives the number of elements in the list.

---

## 6. **List Comprehension:**
Learn how to create new lists using expressions applied to existing lists.

- **Examples:**
  - `[x for x in range(1, 11)]` creates a list of numbers from 1 to 10.
  - `[x * 2 for x in [1, 2, 3]]` results in `[2, 4, 6]`.

---

## 7. **Traversing Lists:**
Explore different ways to traverse lists: item-wise and index-wise.

- **Item-wise Traversal:**
  - Example: `for item in my_list: print(item)`.

- **Index-wise Traversal:**
  - Example: `for i in range(len(my_list)): print(my_list[i])`.

---

## 8. **Zip Function:**
Learn about the `zip()` function to combine multiple iterables into a single iterator of tuples.

- **Example:**
  - `list(zip([1, 2], ['a', 'b']))` results in `[(1, 'a'), (2, 'b')]`.

---

## 9. **Problem Solving:**
This section presents various problems to help practice basic algorithmic challenges and Python concepts.

- **Problem 1: Sequence Sum Calculation**
  - Calculate the sum of the sequence \(\{1/1! + 2/2! + 3/3! + ----- + n/n!}\) for a given integer `n`.

- **Problem 2: Nested Loops for Unique Pairs**
  - Print unique pairs `(i, j)` where `i != j` for `i` and `j` in the range `n`.

- **Problem 3: Pattern Printing**
  - Print various patterns such as asterisks (`*`) and numeric patterns using nested loops.

- **Problem 4: Loop Control Statements (Break, Continue, Pass)**
  - Demonstrate the use of the `break`, `continue`, and `pass` statements in loops with practical examples.

- **Problem 5: Prime Numbers Finder**
  - Find and print all prime numbers within a given range.

- **Problem 6: String Operations**
  - Perform various string manipulations such as slicing, searching, and formatting using built-in Python string functions.

- **Problem 7: Symmetrical String Check**
  - Check if a given string is symmetrical (i.e., both halves of the string are identical).

- **Problem 8: Reverse Words in a String**
  - Reverse the order of words in a given string.

- **Problem 9: Uncommon Words from Two Strings**
  - Find and return the uncommon words between two given strings.

- **Problem 10: Word Location in a String**
  - Find the location (index) of a specific word in a sentence.

- **Problem 11: Remove Duplicate Characters from a String**
  - Remove all duplicate characters from a string while retaining the first occurrence of each character.

- **Problem 12: Append Second String in the Middle of First String**
  - Insert the second string into the middle of the first string at the appropriate position.

- **Problem 13: Sort Characters in a String**
  - Sort the characters of a string in ascending order.

- **Problem 14: Check if a String is Symmetrical**
  - Determine whether the string is symmetrical by checking if both halves of the string are equal.

---

This repository serves as a practical guide for anyone looking to strengthen their problem-solving and Python programming skills. Each section contains code snippets, explanations, and output to ensure clarity and understanding.

Feel free to explore the examples, contribute improvements, and provide feedback!
