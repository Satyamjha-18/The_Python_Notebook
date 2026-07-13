# 📅 Day 07 - Strings in Python

# What is a String?

A String is a sequence of characters enclosed within single quotes (' '), double quotes (" "), or triple quotes.

Example

```python
name = "Satyam"
language = 'Python'
```

---

# Features of Strings

- Ordered
- Immutable
- Supports Indexing
- Supports Slicing
- Allows Duplicate Characters

---

# Creating Strings

```python
name = "Python"

city = 'Patna'

text = """Welcome to Python"""
```

---

# String Indexing

```
P  y  t  h  o  n
0  1  2  3  4  5
```

```python
text = "Python"

print(text[0])

print(text[5])
```

---

# Negative Indexing

```
P  y  t  h  o  n
-6 -5 -4 -3 -2 -1
```

```python
print(text[-1])

print(text[-3])
```

---

# String Slicing

Syntax

```python
string[start:end:step]
```

Example

```python
text = "Python Programming"

print(text[0:6])

print(text[7:18])

print(text[::-1])
```

---

# String Concatenation

```python
first = "Hello"

second = "World"

print(first + " " + second)
```

---

# String Repetition

```python
print("Python " * 3)
```

---

# Membership Operators

```python
print("P" in "Python")

print("Java" not in "Python")
```

---

# Escape Characters

| Escape | Meaning |
|---------|----------|
| \n | New Line |
| \t | Tab |
| \\ | Backslash |
| \' | Single Quote |
| \" | Double Quote |

---

# Common String Methods

| Method | Description |
|---------|-------------|
| upper() | Uppercase |
| lower() | Lowercase |
| title() | Title Case |
| capitalize() | Capitalize First Letter |
| strip() | Remove Spaces |
| replace() | Replace Text |
| split() | Convert to List |
| join() | Join Strings |
| find() | Find Position |
| count() | Count Characters |
| startswith() | Starts With |
| endswith() | Ends With |

---

# String Formatting

Using format()

```python
name = "Satyam"

print("Hello {}".format(name))
```

Using f-string

```python
name = "Satyam"

print(f"Hello {name}")
```

---

# Difference Between List and String

| List | String |
|------|---------|
| Mutable | Immutable |
| [] | Quotes |
| Multiple Data Types | Characters |

---

# Summary

✔ String

✔ Indexing

✔ Slicing

✔ Methods

✔ Formatting

✔ f-Strings

✔ Escape Characters

✔ Interview Questions

---

🎉 Day 07 Completed Successfully 🚀