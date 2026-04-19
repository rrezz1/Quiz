# Python Beginner Quiz

A beginner-friendly quiz to test your basic Python knowledge.

**Total questions:** 15

---

## Questions

### 1. What is the output of: print(type(42))?

- A. `<class 'int'>`
- B. `<class 'str'>`
- C. `<class 'float'>`
- D. `<type 'integer'>`

**Answer:** A

**Explanation:** 42 is an integer literal, so type() returns <class 'int'>.

---

### 2. Which of the following is a valid Python variable name?

- A. `2name`
- B. `my-name`
- C. `my_name`
- D. `class`

**Answer:** C

**Explanation:** Variable names cannot start with a digit, contain hyphens, or be reserved keywords like 'class'.

---

### 3. What does this code print? x = [1, 2, 3]; print(x[1])

- A. `1`
- B. `2`
- C. `3`
- D. `Error`

**Answer:** B

**Explanation:** Python lists are 0-indexed, so index 1 refers to the second element: 2.

---

### 4. How do you write a single-line comment in Python?

- A. `// This is a comment`
- B. `# This is a comment`
- C. `/* This is a comment */`
- D. `-- This is a comment`

**Answer:** B

**Explanation:** Python uses the # symbol to start a single-line comment.

---

### 5. What is the result of 10 % 3?

- A. `3`
- B. `3.33`
- C. `0`
- D. `1`

**Answer:** D

**Explanation:** The % operator returns the remainder of division. 10 / 3 = 3 remainder 1.

---

### 6. Which keyword is used to define a function in Python?

- A. `function`
- B. `fun`
- C. `def`
- D. `define`

**Answer:** C

**Explanation:** The 'def' keyword is used to define a function in Python.

---

### 7. What is the output of: print('5' + '3')?

- A. `8`
- B. `8.0`
- C. `'53'`
- D. `53`

**Answer:** D

**Explanation:** Adding two strings concatenates them. '5' + '3' = '53', not 8.

---

### 8. How do you check if a key 'name' exists in a dictionary d?

- A. `d.has('name')`
- B. `d.contains('name')`
- C. `'name' in d`
- D. `d.exists('name')`

**Answer:** C

**Explanation:** The 'in' operator is used to check for key membership in a dictionary.

---

### 9. What is the output of: len([1, [2, 3], 4])?

- A. `4`
- B. `3`
- C. `2`
- D. `Error`

**Answer:** B

**Explanation:** len() counts top-level elements only. The list has 3 items: 1, [2,3], and 4.

---

### 10. Which loop keeps running as long as a condition is True?

- A. `for loop`
- B. `do-while loop`
- C. `repeat loop`
- D. `while loop`

**Answer:** D

**Explanation:** A while loop repeats its body as long as its condition evaluates to True.

---

### 11. What keyword is used to handle exceptions in Python?

- A. `catch`
- B. `except`
- C. `handle`
- D. `error`

**Answer:** B

**Explanation:** Python uses 'try' and 'except' blocks to handle exceptions.

---

### 12. What is the correct way to create an empty list in Python?

- A. `list = {}`
- B. `list = ()`
- C. `list = []`
- D. `list = <>`

**Answer:** C

**Explanation:** An empty list is created using square brackets: [].

---

### 13. What does the 'return' keyword do in a function?

- A. `Exits the program`
- B. `Prints a value to the screen`
- C. `Sends a value back to the caller`
- D. `Repeats the function`

**Answer:** C

**Explanation:** 'return' sends a value back to wherever the function was called from.

---

### 14. What is the output of: print(bool(0))?

- A. `0`
- B. `True`
- C. `False`
- D. `None`

**Answer:** C

**Explanation:** In Python, 0 is falsy. bool(0) evaluates to False.

---

### 15. Which method adds an item to the end of a list?

- A. `list.add(item)`
- B. `list.push(item)`
- C. `list.insert(item)`
- D. `list.append(item)`

**Answer:** D

**Explanation:** The append() method adds an item to the end of a list.

---

*Quiz source: python_beginner_quiz.json*
