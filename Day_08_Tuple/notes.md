# 📅 Day 08 - Functions in Python

# What is a Function?

A function is a reusable block of code that performs a specific task. Instead of writing the same code repeatedly, we define it once and call it whenever required.

---

# Why Do We Use Functions?

Functions help us:

- Reuse code
- Reduce code duplication
- Improve readability
- Make programs modular
- Simplify debugging and maintenance

---

# Creating a Function

### Syntax

```python
def function_name():
    # Function body
```

### Example

```python
def greet():
    print("Hello, Welcome to Python!")
```

---

# Calling a Function

```python
greet()
```

---

# Function with Parameters

Parameters are variables defined in the function declaration.

```python
def greet(name):
    print("Hello", name)

greet("Satyam")
```

---

# Function with Multiple Parameters

```python
def add(a, b):
    print(a + b)

add(10, 20)
```

---

# Return Statement

The `return` keyword sends the result back to the caller.

```python
def square(num):
    return num * num

result = square(5)
print(result)
```

---

# Types of Arguments

## 1. Positional Arguments

Arguments are passed in the same order as parameters.

```python
def student(name, age):
    print(name, age)

student("Satyam", 22)
```

---

## 2. Keyword Arguments

Arguments are passed using parameter names.

```python
student(age=22, name="Satyam")
```

---

## 3. Default Arguments

A default value is used if no argument is provided.

```python
def country(name="India"):
    print(name)

country()
country("Japan")
```

---

## 4. Variable-Length Arguments (*args)

Used when the number of arguments is unknown.

```python
def total(*numbers):
    print(sum(numbers))

total(10, 20, 30)
```

---

## 5. Keyword Variable-Length Arguments (**kwargs)

Used to pass multiple keyword arguments.

```python
def details(**info):
    print(info)

details(name="Satyam", age=22)
```

---

# Variable Scope

## Local Variable

A variable declared inside a function.

```python
def demo():
    x = 10
    print(x)
```

---

## Global Variable

A variable declared outside the function.

```python
x = 100

def demo():
    print(x)
```

---

# Lambda Function

A lambda function is a small anonymous function.

```python
square = lambda x: x * x

print(square(5))
```

---

# Recursion

Recursion is a process where a function calls itself.

```python
def factorial(n):

    if n == 1:
        return 1

    return n * factorial(n - 1)

print(factorial(5))
```

---

# Built-in Functions

Some commonly used built-in functions:

- print()
- len()
- type()
- sum()
- max()
- min()
- abs()
- round()

---

# Difference Between Parameters and Arguments

| Parameter | Argument |
|-----------|----------|
| Defined in function | Passed during function call |
| Placeholder | Actual value |

Example:

```python
def greet(name):      # Parameter
    print(name)

greet("Satyam")       # Argument
```

---

# Advantages of Functions

- Code Reusability
- Better Code Organization
- Easy Maintenance
- Reduced Code Duplication
- Improved Readability

---

# Summary

✔ What is a Function?

✔ Function Syntax

✔ Function Call

✔ Parameters

✔ Arguments

✔ Return Statement

✔ Default Arguments

✔ Keyword Arguments

✔ Positional Arguments

✔ *args

✔ **kwargs

✔ Local Variable

✔ Global Variable

✔ Lambda Function

✔ Recursion

✔ Built-in Functions

---

# Interview Questions

1. What is a function in Python?
2. Why do we use functions?
3. What is the difference between parameters and arguments?
4. What is the purpose of the `return` statement?
5. What is the difference between local and global variables?
6. Explain `*args` and `**kwargs`.
7. What is a lambda function?
8. What is recursion?
9. What are built-in functions?
10. What are the advantages of using functions?

---

🎉 Day 08 Completed Successfully 🚀