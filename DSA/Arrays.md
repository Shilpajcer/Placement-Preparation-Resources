# 📌 DSA – Arrays

Arrays are one of the most commonly used data structures in coding interviews.

This section contains basic array problems with explanations, examples, and Python solutions.

---

## 1️⃣ Find the Largest Element

### 📝 Problem

Given an array of integers, find the largest element.

### 📌 Example

**Input:**
```text
[10, 25, 7, 42, 18]
```

**Output:**
```text
42
```

### 💡 Approach

1. Assume the first element is the largest.
2. Compare it with every other element.
3. If a larger element is found, update the largest value.

### 💻 Python Solution

```python
arr = [10, 25, 7, 42, 18]

largest = arr[0]

for num in arr:
    if num > largest:
        largest = num

print(largest)
```

**Time Complexity:** `O(n)`  
**Space Complexity:** `O(1)`

---

## 2️⃣ Find the Smallest Element

### 📝 Problem

Given an array of integers, find the smallest element.

### 📌 Example

**Input:**
```text
[10, 25, 7, 42, 18]
```

**Output:**
```text
7
```

### 💡 Approach

1. Assume the first element is the smallest.
2. Compare it with every other element.
3. Update the value whenever a smaller element is found.

### 💻 Python Solution

```python
arr = [10, 25, 7, 42, 18]

smallest = arr[0]

for num in arr:
    if num < smallest:
        smallest = num

print(smallest)
```

**Time Complexity:** `O(n)`  
**Space Complexity:** `O(1)`

---

## 3️⃣ Find the Sum of Array Elements

### 📝 Problem

Find the sum of all elements in an array.

### 📌 Example

**Input:**
```text
[1, 2, 3, 4, 5]
```

**Output:**
```text
15
```

### 💡 Approach

Start with `0` and add each element to the total.

### 💻 Python Solution

```python
arr = [1, 2, 3, 4, 5]

total = 0

for num in arr:
    total += num

print(total)
```

**Time Complexity:** `O(n)`  
**Space Complexity:** `O(1)`

---

## 4️⃣ Count Even Numbers

### 📝 Problem

Count the number of even elements in an array.

### 📌 Example

**Input:**
```text
[1, 2, 4, 7, 8, 9]
```

**Output:**
```text
3
```

### 💡 Approach

An even number is divisible by `2`.

```python
num % 2 == 0
```

### 💻 Python Solution

```python
arr = [1, 2, 4, 7, 8, 9]

count = 0

for num in arr:
    if num % 2 == 0:
        count += 1

print(count)
```

**Time Complexity:** `O(n)`  
**Space Complexity:** `O(1)`

---

## 5️⃣ Reverse an Array

### 📝 Problem

Reverse the elements of an array.

### 📌 Example

**Input:**
```text
[1, 2, 3, 4, 5]
```

**Output:**
```text
[5, 4, 3, 2, 1]
```

### 💡 Approach

Use Python's `reverse()` method to reverse the array.

### 💻 Python Solution

```python
arr = [1, 2, 3, 4, 5]

arr.reverse()

print(arr)
```

**Time Complexity:** `O(n)`  
**Space Complexity:** `O(1)`

---

## 📚 More Problems to Practice

- Find the second largest element
- Remove duplicates from an array
- Find the frequency of each element
- Find the missing number
- Move all zeros to the end
- Find duplicate elements
- Find the sum of positive and negative numbers
- Find the maximum difference between two elements

---

⭐ More DSA problems will be added as I continue my placement preparation.
