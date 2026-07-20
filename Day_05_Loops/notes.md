# 📅 Day 05 - Loops in Python

# What is a Loop?

A loop is a programming structure that repeats a block of code until a condition becomes False or until all items in a sequence are processed.

Loops help us avoid writing the same code multiple times.

---

# Why Do We Use Loops?

Without loops:

```python
print("Hello")
print("Hello")
print("Hello")
print("Hello")
print("Hello")
```

With loops:

```python
for i in range(5):
    print("Hello")
```

---

# Types of Loops in Python

Python provides two types of loops:

- for Loop
- while Loop

---

# 1. for Loop

The `for` loop is used to iterate over a sequence such as a list, tuple, string, or range.

### Syntax

```python
for variable in sequence:
    statements
```

### Example

```python
for i in range(5):
    print(i)
```

Output

```
0
1
2
3
4
```

---

# range() Function

The `range()` function generates a sequence of numbers.

```python
range(stop)
range(start, stop)
range(start, stop, step)
```

Examples

```python
range(5)
range(1, 6)
range(1, 11, 2)
```

---

# 2. while Loop

A `while` loop executes as long as its condition remains `True`.

### Syntax

```python
while condition:
    statements
```

Example

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

---

# Nested Loops

A loop inside another loop is called a nested loop.

```python
for i in range(3):
    for j in range(3):
        print(i, j)
```

---

# break Statement

Stops the loop immediately.

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

---

# continue Statement

Skips the current iteration and moves to the next one.

```python
for i in range(6):
    if i == 3:
        continue
    print(i)
```

---

# pass Statement

Used as a placeholder when no action is required.

```python
for i in range(5):
    if i == 3:
        pass
    print(i)
```

---

# Infinite Loop

while True:
    print("Hello")
```

Use carefully because it never stops unless interrupted.

---

# Difference Between for and while

|            for Loop                |          while Loop                 |
|------------------------------------|-------------------------------------|
| Used for sequences                 | Used for conditions                 |
| Number of iterations usually known | Number of iterations may be unknown |

---

# Interview Questions

### What is a loop?

A loop repeatedly executes a block of code until a condition changes.

---

### Difference between for and while?

`for` is generally used for iterating over sequences, while `while` runs based on a condition.

---

### What is break?

`break` terminates the loop immediately.

---

### What is continue?

`continue` skips the current iteration.

---

### What is pass?

`pass` is a placeholder that does nothing.

---

# Summary

✔ for Loop

✔ while Loop

✔ range()

✔ Nested Loop

✔ break

✔ continue

✔ pass

✔ Infinite Loop

✔ Interview Questions

---

🎉 Day 05 Completed Successfully 🚀