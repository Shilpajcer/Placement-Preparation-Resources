# 🐍 Python Interview Questions for Freshers

A beginner-friendly Python interview guide covering important concepts and common placement questions.

---

## 1. Python Basics

### Q1. What is Python?

Python is a high-level, interpreted, general-purpose programming language known for its simple and readable syntax.

### Q2. What are the features of Python?

- Easy to learn and read
- Interpreted
- Dynamically typed
- Object-oriented
- Large standard library
- Supports multiple programming paradigms
- Cross-platform

### Q3. What is a variable?

A variable is a name used to refer to a value.

Example:

    age = 21
    name = "Shilpa"

### Q4. What are common Python data types?

- `int` → Integer
- `float` → Decimal number
- `str` → String
- `bool` → True or False
- `list` → Ordered, changeable collection
- `tuple` → Ordered, unchangeable collection
- `set` → Unordered collection of unique values
- `dict` → Key-value pairs

---

# 2. List, Tuple, Set and Dictionary

## List

A list is an ordered and mutable collection.

Example:

    numbers = [10, 20, 30, 40]

Lists allow duplicate values.

## Tuple

A tuple is an ordered and immutable collection.

Example:

    numbers = (10, 20, 30, 40)

## Set

A set stores unique values.

Example:

    numbers = {10, 20, 30, 40}

Duplicate values are automatically removed.

## Dictionary

A dictionary stores data as key-value pairs.

Example:

    student = {
        "name": "Shilpa",
        "age": 21
    }

---

## List vs Tuple

| List | Tuple |
|---|---|
| Mutable | Immutable |
| Uses `[]` | Uses `()` |
| Can be modified | Cannot be modified |
| Generally more flexible | Generally more memory-efficient |

---

# 3. Strings

### Q1. What is a string?

A string is a sequence of characters.

Example:

    name = "Python"

### Q2. How do you reverse a string?

    text = "Python"
    reverse = text[::-1]

### Q3. How do you check whether a string is a palindrome?

A palindrome reads the same forward and backward.

Example:

    text = "madam"

    if text == text[::-1]:
        print("Palindrome")

### Common String Methods

- `lower()`
- `upper()`
- `strip()`
- `replace()`
- `split()`
- `find()`
- `count()`

---

# 4. Conditional Statements

Python uses `if`, `elif`, and `else` for decision making.

Example:

    age = 20

    if age >= 18:
        print("Adult")
    else:
        print("Minor")

### Common Interview Questions

- Check whether a number is even or odd.
- Find the largest of two numbers.
- Find the largest of three numbers.
- Check whether a year is a leap year.
- Check whether a number is positive, negative, or zero.

---

# 5. Loops

Loops are used to execute a block of code repeatedly.

## For Loop

Used when iterating over a sequence or a known range.

Example:

    for i in range(1, 6):
        print(i)

## While Loop

Runs while a condition is true.

Example:

    i = 1

    while i <= 5:
        print(i)
        i += 1

---

## Break vs Continue

### `break`

Stops the loop completely.

### `continue`

Skips the current iteration and moves to the next iteration.

---

# 6. Functions

A function is a reusable block of code that performs a specific task.

Example:

    def add(a, b):
        return a + b

### Why use functions?

- Code reusability
- Better organization
- Easier debugging
- Reduces repetition

### Parameters vs Arguments

**Parameter:** Variable written in the function definition.

**Argument:** Actual value passed to the function.

Example:

    def add(a, b):
        return a + b

    add(10, 20)

Here `a` and `b` are parameters, while `10` and `20` are arguments.

---

# 7. Object-Oriented Programming

Python supports Object-Oriented Programming.

The four main principles are:

1. Encapsulation
2. Abstraction
3. Inheritance
4. Polymorphism

### Q1. What is a class?

A class is a blueprint for creating objects.

### Q2. What is an object?

An object is an instance of a class.

Example:

    class Student:
        def __init__(self, name):
            self.name = name

    student1 = Student("Shilpa")

Here `Student` is the class and `student1` is an object.

### Q3. What is `self`?

`self` refers to the current object of the class.

### Q4. What is `__init__()`?

`__init__()` is a special method that is automatically called when an object is created. It is commonly used to initialize object data.

---

# 8. Inheritance

Inheritance allows a child class to acquire properties and methods from a parent class.

Example:

    class Animal:
        def sound(self):
            print("Animal makes a sound")

    class Dog(Animal):
        pass

Here `Dog` inherits from `Animal`.

### Types of inheritance

- Single inheritance
- Multiple inheritance
- Multilevel inheritance
- Hierarchical inheritance

---

# 9. Polymorphism

Polymorphism means the same operation can behave differently depending on the object or situation.

Example:

    class Dog:
        def sound(self):
            print("Bark")

    class Cat:
        def sound(self):
            print("Meow")

Both classes have a `sound()` method, but they behave differently.

---

# 10. Exception Handling

Exception handling is used to handle runtime errors without abruptly stopping the program.

Common keywords:

- `try`
- `except`
- `else`
- `finally`

Example:

    try:
        result = 10 / 0
    except ZeroDivisionError:
        print("Cannot divide by zero")

---

# 11. Important Python Concepts

### Mutable vs Immutable

**Mutable objects** can be changed after creation.

Examples:
- List
- Dictionary
- Set

**Immutable objects** cannot be changed after creation.

Examples:
- Integer
- Float
- String
- Tuple

### `==` vs `is`

`==` checks whether two values are equal.

`is` checks whether two references point to the same object.

### `append()` vs `extend()`

`append()` adds one item to a list.

`extend()` adds multiple elements from another iterable.

Example:

    numbers = [1, 2]

    numbers.append(3)
    # [1, 2, 3]

    numbers.extend([4, 5])
    # [1, 2, 3, 4, 5]

---

# 12. Common Python Coding Questions

Practice these questions before interviews:

### Beginner

1. Check whether a number is even or odd.
2. Find the largest of three numbers.
3. Find the factorial of a number.
4. Check whether a number is prime.
5. Check whether a number is a palindrome.
6. Reverse a number.
7. Find the sum of digits.
8. Count the number of digits.
9. Check whether a number is an Armstrong number.
10. Check whether a year is a leap year.

### Strings

11. Reverse a string.
12. Check whether a string is a palindrome.
13. Count vowels in a string.
14. Count characters in a string.
15. Find the frequency of each character.
16. Remove spaces from a string.
17. Check whether two strings are anagrams.

### Arrays / Lists

18. Find the largest element.
19. Find the smallest element.
20. Find the second largest element.
21. Find the sum of array elements.
22. Count even and odd numbers.
23. Remove duplicates.
24. Reverse an array.
25. Move all zeroes to the end.
26. Find duplicate elements.
27. Search for an element.

---

# 13. Frequently Asked Python Interview Questions

### Q1. Is Python compiled or interpreted?

Python is generally described as an interpreted language. Python source code is first converted into bytecode, which is then executed by the Python interpreter.

### Q2. What is dynamic typing?

In Python, you do not need to explicitly declare the variable's data type.

Example:

    x = 10
    x = "Python"

The same variable can refer to values of different types at different times.

### Q3. What is indentation in Python?

Indentation is used to define blocks of code in Python.

Example:

    if x > 0:
        print("Positive")

### Q4. What is a module?

A module is a Python file containing code such as functions, classes, or variables that can be imported into another program.

### Q5. What is a package?

A package is a collection of related Python modules organized together.

### Q6. What is a lambda function?

A lambda is a small anonymous function written using the `lambda` keyword.

Example:

    square = lambda x: x * x

### Q7. What is list comprehension?

List comprehension provides a short way to create a list.

Example:

    squares = [x * x for x in range(1, 6)]

---

# 14. Python Interview Quick Revision

| Topic | Remember |
|---|---|
| Variable | Stores/reference a value |
| List | Ordered and mutable |
| Tuple | Ordered and immutable |
| Set | Unique values |
| Dictionary | Key-value pairs |
| String | Sequence of characters |
| Function | Reusable block of code |
| Class | Blueprint for objects |
| Object | Instance of a class |
| Inheritance | Reuse properties and methods |
| Polymorphism | Different behavior through common interface |
| Exception Handling | Handles runtime errors |
| `==` | Compares values |
| `is` | Checks object identity |

---

# 🎯 Placement Preparation Tips

- Learn Python fundamentals before advanced topics.
- Practice coding without copying solutions.
- Understand the logic before memorizing syntax.
- Be ready to explain every project written on your resume.
- Practice arrays and strings regularly.
- Revise OOP concepts before technical interviews.
- Do not mention Python topics on your resume that you cannot explain.
- Practice writing code by hand because some interviews use coding tests.

> **Learn the concept → Understand the logic → Write the code → Practice → Explain it confidently 🚀**
