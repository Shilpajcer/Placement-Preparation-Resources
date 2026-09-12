# 📌 DSA – Arrays

Arrays are one of the most commonly used data structures in coding interviews.

This section contains basic array problems with explanations, examples, and Python solutions.

---

## 1️⃣ Find the Largest Element

### Problem
Given an array of integers, find the largest element.

### Example

**Input:**
```text
[10, 25, 7, 42, 18]
Output:

42
Approach
Assume the first element is the largest.
Compare it with every other element.
If a larger element is found, update the largest value.
Python Solution
arr = [10, 25, 7, 42, 18]

largest = arr[0]

for num in arr:
    if num > largest:
        largest = num

print(largest)

Time Complexity: O(n)
Space Complexity: O(1)

## 2️⃣ Find the Smallest Element
###Problem

Given an array of integers, find the smallest element.

Example

**Input:**

[10, 25, 7, 42, 18]

Output:

7
Approach
Assume the first element is the smallest.
Compare it with every other element.
Update the value whenever a smaller element is found.
Python Solution
arr = [10, 25, 7, 42, 18]

smallest = arr[0]

for num in arr:
    if num < smallest:
        smallest = num

print(smallest)

Time Complexity: O(n)
Space Complexity: O(1)

## 3️⃣ Find the Sum of Array Elements
###Problem

Find the sum of all elements in an array.

Example

**Input:**

[1, 2, 3, 4, 5]

Output:

15
Approach

Start with 0 and add each element to the total.

Python Solution
arr = [1, 2, 3, 4, 5]

total = 0

for num in arr:
    total += num

print(total)

Time Complexity: O(n)
Space Complexity: O(1)

## 4️⃣ Count Even Numbers
###Problem

Count the number of even elements in an array.

Example

**Input:**

[1, 2, 4, 7, 8, 9]

Output:

3
Approach

An even number is divisible by 2.

num % 2 == 0
Python Solution
arr = [1, 2, 4, 7, 8, 9]

count = 0

for num in arr:
    if num % 2 == 0:
        count += 1

print(count)

Time Complexity: O(n)
Space Complexity: O(1)

## 5️⃣ Reverse an Array
###Problem

Reverse the elements of an array.

Example

**Input:**

[1, 2, 3, 4, 5]

Output:

[5, 4, 3, 2, 1]
Python Solution
arr = [1, 2, 3, 4, 5]

arr.reverse()

print(arr)

Time Complexity: O(n)
Space Complexity: O(1)
