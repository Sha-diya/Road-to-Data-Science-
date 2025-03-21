# Python Fundamentals: Day 04

## Overview

This Jupyter Notebook, titled "Day_04.ipynb," is part of the "Python Fundamentals" series and focuses on the topic of lists in Python. It covers various aspects of lists, including their creation, modification, operations, and advanced techniques like list comprehensions.

## Table of Contents

1. [Introduction to Lists](#introduction-to-lists)
2. [Characteristics of Lists](#characteristics-of-lists)
3. [Creating Lists](#creating-lists)
4. [Accessing List Items](#accessing-list-items)
5. [Modifying Lists](#modifying-lists)
6. [Deleting Items from Lists](#deleting-items-from-lists)
7. [Operations on Lists](#operations-on-lists)
8. [List Functions](#list-functions)
9. [List Comprehension](#list-comprehension)
10. [Traversing Lists](#traversing-lists)
11. [Using `zip()`](#using-zip)
12. [Solved Problems](#solved-problems)

## Introduction to Lists

- Definition and uses of lists.
- Comparison between lists and arrays, highlighting differences in size, homogeneity, speed, and memory usage.

**Problem**: Create a list of your favorite fruits and print it.

## Characteristics of Lists

- Lists are ordered, mutable, heterogeneous, can have duplicates, are dynamic, and can be nested.

**Problem**: Create a list with different data types (integer, string, float, and boolean) and print each item with its type.

## Creating Lists

- Methods to create empty, one-dimensional, two-dimensional, three-dimensional, and heterogeneous lists.
- Type conversion to create lists.

**Problem**: Create a two-dimensional list representing a matrix and print it.

## Accessing List Items

- Indexing and slicing techniques to access items from lists.
- Positive and negative indexing, and nested list indexing.

**Problem**: Access and print the third item from a list of numbers using both positive and negative indexing.

## Modifying Lists

- Various ways to add items using append, extend, and insert.
- Editing items using indexing and slicing.

**Problem**: Add a new item to a list of colors using the append method, then insert another item at the second position.

## Deleting Items from Lists

- Using `del`, `remove`, `pop`, and `clear` to delete items from lists.

**Problem**: Remove an item from a list of animals by its value and another item by its index.

## Operations on Lists

- Arithmetic operations (`+`, `*`), membership operations, and loops to iterate over lists.

**Problem**: Concatenate two lists of numbers and print the result. Then, check if a specific number is present in the concatenated list.

## List Functions

- Built-in functions such as `len()`, `min()`, `max()`, `sorted()`, `count()`, `index()`, `reverse()`, `sort()`, and `copy()`.

**Problem**: Find the length, minimum, maximum, and sorted version of a list of random numbers.

## List Comprehension

- Explanation and examples of list comprehension for concise list creation.
- Examples include creating lists, scalar multiplication, generating squares, filtering lists by conditions, and nested comprehensions.

**Problem**: Use list comprehension to create a list of squares of numbers from 1 to 10.

## Traversing Lists

- Item-wise and index-wise traversal of lists.

**Problem**: Write a loop to print each item in a list of countries.

## Using `zip()`

- Explanation of the `zip()` function and how to use it to combine items from multiple lists index-wise.

**Problem**: Use the `zip()` function to combine two lists of equal length into a list of tuples.

## Solved Problems

1. **Create a List of Favorite Fruits**:
   ```python
   fruits = ["apple", "banana", "cherry"]
   print(fruits)
2. **Create a List with Different Data Types:**
   ```python
   mixed_list = [10, "hello", 3.14, True]
   for item in mixed_list:
     print(f"{item} is of type {type(item)}")
3. **Create a Two-Dimensional List Representing a Matrix:**
   ```python
    matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
    print(matrix)
4. **Access and Print the Third Item from a List:**
   ```python
   numbers = [10, 20, 30, 40, 50]
   print(numbers[2])  # Positive indexing
   print(numbers[-3])  # Negative indexing
5. **Add Items to a List of Colors Using Append and Insert:**
   ```python
   colors = ["red", "green", "blue"]
   colors.append("yellow")
   colors.insert(1, "orange")
   print(colors)
6. **Remove Items from a List of Animals:**
   ```python
   animals = ["cat", "dog", "rabbit", "hamster"]
   animals.remove("rabbit")
   del animals[1]
   print(animals)
7. **Concatenate Two Lists and Check Membership:**
   ```python
   list1 = [1, 2, 3]
   list2 = [4, 5, 6]
   combined_list = list1 + list2
   print(combined_list)
   print(5 in combined_list)
8. **Find Length, Minimum, Maximum, and Sorted Version of a List:**
   ```python
   random_numbers = [23, 1, 45, 34, 7]
   print(len(random_numbers))
   print(min(random_numbers))
   print(max(random_numbers))
   print(sorted(random_numbers))
9. **Use List Comprehension to Create a List of Squares:**
    ```python
    squares = [x**2 for x in range(1, 11)]
    print(squares)
10. **Print Each Item in a List of Countries:**
    ```python
    countries = ["USA", "Canada", "Germany", "France"]
    for country in countries:
      print(country)
11. **Use zip() to Combine Two Lists into a List of Tuples:**
    ```python
    list1 = [1, 2, 3]
    list2 = ['a', 'b', 'c']
    combined = list(zip(list1, list2))
    print(combined)
