# 💻 DSA – Strings

A beginner-friendly collection of important string concepts, operations, and placement practice questions.

## 📌 What is a String?

A string is a sequence of characters.

Examples: `"hello"`, `"placement"`, `"python"`

In Python, strings are written inside single or double quotes.

---

## 🔹 Basic String Operations

### 1. Find Length

`len("hello")` → `5`

### 2. Access Characters

`text[0]` → First character  
`text[-1]` → Last character

Example: `"hello"[0]` → `h`

### 3. Convert to Uppercase

`"hello".upper()` → `HELLO`

### 4. Convert to Lowercase

`"HELLO".lower()` → `hello`

### 5. Reverse a String

`"hello"[::-1]` → `olleh`

---

# 🎯 Important Placement Questions

## 1️⃣ Reverse a String

**Problem:** Reverse the given string.

**Example:**  
Input: `hello`  
Output: `olleh`

**Python:**

    text = input()
    print(text[::-1])

**Concept:** `[::-1]` reads the string from the last character to the first.

---

## 2️⃣ Check Palindrome

**Problem:** Check whether a string reads the same forward and backward.

**Example:**  
Input: `madam`  
Output: `Palindrome`

**Python:**

    text = input()

    if text == text[::-1]:
        print("Palindrome")
    else:
        print("Not Palindrome")

**Examples:** `madam`, `level`, `radar`

---

## 3️⃣ Count Vowels

**Problem:** Count the number of vowels in a string.

**Example:**  
Input: `education`  
Output: `5`

**Python:**

    text = input()
    count = 0

    for ch in text:
        if ch.lower() in "aeiou":
            count += 1

    print(count)

---

## 4️⃣ Count Characters Without Using len()

**Problem:** Find the length of a string without using `len()`.

**Python:**

    text = input()
    count = 0

    for ch in text:
        count += 1

    print(count)

---

## 5️⃣ Count Frequency of a Character

**Problem:** Count how many times a particular character occurs.

**Example:**  
Input: `banana`  
Character: `a`  
Output: `3`

**Python:**

    text = input()
    target = input()

    count = 0

    for ch in text:
        if ch == target:
            count += 1

    print(count)

---

## 6️⃣ Remove Spaces

**Problem:** Remove all spaces from a string.

**Example:**  
Input: `hello world`  
Output: `helloworld`

**Python:**

    text = input()
    print(text.replace(" ", ""))

---

## 7️⃣ Check Anagram

**Problem:** Check whether two strings contain the same characters with the same frequency.

**Example:**  
`listen` → `silent`  
Output: `Anagram`

**Python:**

    str1 = input()
    str2 = input()

    if sorted(str1) == sorted(str2):
        print("Anagram")
    else:
        print("Not Anagram")

**Examples:** `listen → silent`, `race → care`

---

# 🧠 Important String Methods

| Method | Purpose |
|---|---|
| `len()` | Find length |
| `upper()` | Convert to uppercase |
| `lower()` | Convert to lowercase |
| `strip()` | Remove spaces from beginning/end |
| `replace()` | Replace characters |
| `split()` | Split a string |
| `join()` | Join strings |
| `find()` | Find position |
| `count()` | Count occurrences |
| `startswith()` | Check starting characters |
| `endswith()` | Check ending characters |

---

# 🚀 Practice Questions

Try solving these yourself:

1. Reverse a string.
2. Check whether a string is a palindrome.
3. Count vowels in a string.
4. Count consonants in a string.
5. Find the length of a string without using `len()`.
6. Count the frequency of a character.
7. Remove spaces from a string.
8. Check whether two strings are anagrams.
9. Find duplicate characters in a string.
10. Find the first non-repeating character.
11. Count the number of words in a sentence.
12. Convert lowercase characters to uppercase.
13. Find the largest word in a sentence.
14. Remove duplicate characters from a string.
15. Check whether a string contains only digits.

---

# 📌 Quick Revision

| Concept | Example |
|---|---|
| Length | `len("hello")` → `5` |
| First Character | `"hello"[0]` → `h` |
| Last Character | `"hello"[-1]` → `o` |
| Reverse | `"hello"[::-1]` → `olleh` |
| Uppercase | `"hello".upper()` |
| Lowercase | `"HELLO".lower()` |
| Replace | `"hello".replace("h","H")` |
| Count | `"banana".count("a")` |

---

## 🎯 Placement Tip

For string problems, think:

**Input → Characters → Condition → Count/Store → Output**

Start with basic problems and gradually move to frequency counting, duplicates, anagrams, and interview-level problems.

---

⭐ More DSA string problems and solutions will be added as the repository grows.
