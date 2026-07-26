# 📘 Day 09 - Dictionary in Python

# What is a Dictionary?

A dictionary is a mutable collection of data stored as **key-value pairs**.

- Mutable
- Ordered (Python 3.7+)
- No duplicate keys
- Fast lookup using keys

Example:

```python
student = {
    "name": "Satyam",
    "age": 22,
    "city": "Patna"
}
```

---

# Characteristics of Dictionary

✔ Stores data as key-value pairs

✔ Mutable

✔ Ordered (Python 3.7+)

✔ Keys must be unique

✔ Values can be duplicated

✔ Keys must be immutable (string, int, tuple, etc.)

---

# Creating a Dictionary

```python
student = {
    "name": "Satyam",
    "age": 22,
    "course": "Python"
}
```

---

# Empty Dictionary

```python
d = {}

# OR

d = dict()
```

---

# Accessing Values

```python
print(student["name"])

print(student.get("age"))
```

> `get()` returns `None` if the key does not exist, avoiding a `KeyError`.

---

# Adding Items

```python
student["city"] = "Patna"

print(student)
```

---

# Updating Items

```python
student["age"] = 23

print(student)
```

---

# Deleting Items

## Using del

```python
del student["age"]
```

## Using pop()

```python
student.pop("city")
```

## Using popitem()

```python
student.popitem()
```

## Using clear()

```python
student.clear()
```

---

# Dictionary Methods

## keys()

```python
print(student.keys())
```

## values()

```python
print(student.values())
```

## items()

```python
print(student.items())
```

## update()

```python
student.update({"age": 24})
```

## copy()

```python
new_student = student.copy()
```

---

# Looping Through Dictionary

## Loop through keys

```python
for key in student:
    print(key)
```

## Loop through values

```python
for value in student.values():
    print(value)
```

## Loop through key-value pairs

```python
for key, value in student.items():
    print(key, value)
```

---

# Nested Dictionary

```python
students = {
    "student1": {
        "name": "Satyam",
        "age": 22
    },
    "student2": {
        "name": "Rahul",
        "age": 21
    }
}
```

Access:

```python
print(students["student1"]["name"])
```

---

# Dictionary Comprehension

```python
square = {x: x*x for x in range(1,6)}

print(square)
```

Output

```python
{1:1,2:4,3:9,4:16,5:25}
```

---

# Built-in Functions

```python
print(len(student))

print(type(student))

print(sorted(student))
```

---

# Dictionary vs List

| Dictionary | List |
|------------|------|
| Stores key-value pairs | Stores values only |
| Uses {} | Uses [] |
| Keys are unique | Duplicate values allowed |
| Fast lookup by key | Access by index |

---

# Advantages of Dictionary

- Fast searching
- Easy data organization
- Efficient updates
- Flexible data storage
- Supports nested structures

---

# Disadvantages of Dictionary

- More memory usage than lists
- Keys must be unique
- Mutable (data can change)

---

# Summary

✔ Dictionary

✔ Key-Value Pair

✔ Mutable

✔ Ordered

✔ Methods

✔ Looping

✔ Nested Dictionary

✔ Dictionary Comprehension

✔ Built-in Functions

---

# Practice Questions

1. Create a dictionary for a student.
2. Add a new key-value pair.
3. Update an existing value.
4. Delete a key using `del`.
5. Delete a key using `pop()`.
6. Print all keys.
7. Print all values.
8. Loop through a dictionary.
9. Create a nested dictionary.
10. Write a dictionary comprehension.

---

# Interview Questions

1. What is a dictionary in Python?
2. Difference between dictionary and list?
3. Why must dictionary keys be unique?
4. Difference between `get()` and `[]`?
5. Explain `pop()` and `popitem()`.
6. What is dictionary comprehension?
7. What are mutable and immutable keys?
8. Difference between `keys()`, `values()`, and `items()`?
9. Can a dictionary have duplicate values?
10. When should you use a dictionary?

---

🎉 Day 09 Completed Successfully 🚀