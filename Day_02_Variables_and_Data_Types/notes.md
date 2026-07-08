# 📅 Day 02 - Variables, Comments & Data Types

## 📌 Topics Covered

- Variables
- Rules for Variable Declaration
- Naming Conventions
- Comments
- Data
- Data Types
- Type Checking
- Type Casting
- User Input
- Interview Questions

---

# What is a Variable?

A **variable** is a named memory location used to store data. The value stored in a variable can change during the execution of a program.

Python is a **dynamically typed language**, which means you do not need to specify the data type while creating a variable. Python automatically identifies the data type based on the assigned value.

### Syntax

variable_name = value

### Example

x = 5
name = "John"

print(x)
print(name)

Output
5
John


# Rules for Variable Declaration

A valid variable name must follow these rules:

✅ Variable name should start with a letter (A-Z, a-z) or underscore (_)

✅ Variable name cannot start with a number

✅ Spaces are not allowed

✅ Special characters are not allowed except underscore (_)

✅ Variable names are case-sensitive

✅ Reserved keywords cannot be used as variable names


# Variable Naming Examples

| ✅ Valid Variables  | ❌ Invalid Variables |
|       name          | 15name                |
|       city          | Full Name             |
|       age1          | $city                 |
|     Full_Name       | my-name               |
|    student_name     | class                 |

Example

student_name = "Satyam"
age = 22
_city = "Patna"


# Multiple Variable Assignment

Assign same value to multiple variables.

x = y = z = 100

print(x)
print(y)
print(z)
```

Output
100
100
100
```

Assign different values.

name, age, city = "Satyam", 22, "Patna"

print(name)
print(age)
print(city)

---

# Comments in Python

Comments are used to explain code. Python ignores comments while executing the program.

They improve code readability and make it easier for developers to understand the program.

---

## Single Line Comment

Use **#**

```python
# This is a single-line comment

name = "Satyam"
```

---

## Multi-line Comment (Docstring)

Use triple quotes.

```python
"""
This is a
multi-line comment.
"""
```

---

# What is Data?

Data is a collection of facts, values or information that can be processed by a computer.

Example

```
100
45.67
Python
True
```

---

# What is a Data Type?

A **Data Type** defines the type of value stored inside a variable.

Python automatically assigns a data type based on the value.

Example

age = 22
name = "Satyam"

# Basic Data Types

## 1. Integer (int)

Stores whole numbers.

age = 22


## 2. Float (float)

Stores decimal numbers.


price = 99.99

## 3. Complex (complex)

Stores complex numbers.

num = 3 + 5j


## 4. String (str)

Stores text.


name = "Satyam"


## 5. Boolean (bool)

Stores only two values.


True
False


Example

```python
is_student = True
```

---

## 6. List

Ordered and Mutable.

```python
fruits = ["Apple", "Banana", "Mango"]
```

---

## 7. Tuple

Ordered and Immutable.

```python
numbers = (10, 20, 30)
```

---

## 8. Set

Unordered collection of unique values.

```python
colors = {"Red", "Blue", "Green"}
```

---

## 9. Dictionary

Stores data as Key-Value pairs.

```python
student = {
    "Name": "Satyam",
    "Age": 22
}
```

---

# Type Checking

Use **type()** function.

```python
age = 22

print(type(age))
```

Output

```
<class 'int'>
```

---

# Type Casting

Type casting means converting one data type into another.

Convert String to Integer

```python
num = "100"

print(int(num))
```

Convert Integer to Float

```python
price = 25

print(float(price))
```

Convert Integer to String

```python
marks = 95

print(str(marks))
```

---

# Taking User Input

```python
name = input("Enter your name : ")

print("Welcome", name)
```

Example

```
Enter your name : Satyam

Welcome Satyam
```

---

# Useful Built-in Functions

| Function | Description |
|----------|-------------|
| type() | Check Data Type |
| int() | Convert to Integer |
| float() | Convert to Float |
| str() | Convert to String |
| bool() | Convert to Boolean |
| input() | Take User Input |
| len() | Find Length |

---

# Interview Questions

### Q1. What is a Variable?

A variable is a named memory location used to store data.

---

### Q2. What is Data Type?

A data type defines the type of value stored in a variable.

---

### Q3. Why is Python called a Dynamically Typed Language?

Because we do not need to declare the data type of a variable. Python automatically determines it based on the assigned value.

---

### Q4. What is Type Casting?

Type casting is the process of converting one data type into another.

---

### Q5. Difference between int and float?

| int | float |
|------|--------|
| Stores whole numbers | Stores decimal numbers |

---

### Q6. Difference between List and Tuple?

| List | Tuple |
|------|--------|
| Mutable | Immutable |

---

### Q7. Difference between Set and Dictionary?

| Set | Dictionary |
|------|------------|
| Stores unique values | Stores key-value pairs |

---

# Day 02 Summary

✅ Variables

✅ Variable Naming Rules

✅ Multiple Variable Assignment

✅ Comments

✅ Data

✅ Data Types

✅ Type Checking

✅ Type Casting

✅ User Input

✅ Built-in Functions

✅ Interview Questions

---

# 🎯 Key Takeaways

- Variables are used to store data.
- Python is dynamically typed.
- Follow proper variable naming rules.
- Comments improve code readability.
- Python supports multiple built-in data types.
- Use `type()` to identify data types.
- Use type casting to convert one data type into another.

---

**🎉 Day 02 Completed Successfully 🚀**
