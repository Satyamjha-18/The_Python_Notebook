# 📅 Day 08 - Functions in Python

# What is a Function?

A function is a reusable block of code that performs a specific task.

Instead of writing the same code multiple times, we write it once inside a function and call it whenever needed.

---

# Advantages of Functions

- Code Reusability
- Better Readability
- Easy Maintenance
- Reduces Code Duplication
- Modular Programming

---

# Creating a Function

Syntax

```python
def function_name():
    # code
```

Example

```python
def greet():
    print("Hello World")
```

---

# Calling a Function

```python
greet()
```

---

# Function with Parameters

```python
def greet(name):
    print("Hello", name)
```

---

# Function with Multiple Parameters

```python
def add(a, b):
    print(a + b)
```

---

# Return Statement

```python
def square(n):
    return n * n
```

---

# Default Arguments

```python
def country(name="India"):
    print(name)
```

---

# Keyword Arguments

```python
def student(name, age):
    print(name, age)

student(age=22, name="Satyam")
```

---

# Positional Arguments

```python
student("Satyam",22)
```

---

# Variable Length Arguments (*args)

```python
def total(*numbers):
    print(sum(numbers))
```

---

# Keyword Variable Arguments (**kwargs)

```python
def details(**data):
    print(data)
```

---

# Local Variable

Accessible only inside the function.

---

# Global Variable

Accessible throughout the program.

---

# Built-in Functions

Examples:

- len()
- sum()
- max()
- min()
- abs()
- round()
- type()

---

# Lambda Function

```python
square = lambda x: x*x
```

---

# Recursion

A function calling itself.

Example:

```python
def factorial(n):
    if n==1:
        return 1
    return n*factorial(n-1)
```

---

# Summary

✔ Function

✔ Parameters

✔ Arguments

✔ Return

✔ Default Arguments

✔ *args

✔ **kwargs

✔ Scope

✔ Lambda

✔ Recursion

---

🎉 Day 08 Completed Successfully 🚀