# 📘 Day 08 - Tuples in Python

# What is a Tuple?

A tuple is an ordered and immutable collection of items in Python.

- Ordered
- Immutable
- Allows duplicate values
- Supports different data types

Example:

```python
student = ("Satyam", 22, "Python")
```

---

# Characteristics of Tuple

✔ Ordered

✔ Immutable

✔ Allows Duplicates

✔ Faster than List

✔ Can Store Multiple Data Types

---

# Creating Tuples

```python
t1 = (1,2,3)

t2 = ("Python","Java","C++")

t3 = (10,"Satyam",22.5,True)
```

---

# Empty Tuple

```python
t = ()
```

---

# Single Element Tuple

```python
t = (10,)
```

> **Note:** Comma is mandatory for a single-element tuple.

---

# Accessing Elements

```python
fruits = ("Apple","Banana","Mango")

print(fruits[0])

print(fruits[2])
```

---

# Negative Indexing

```python
print(fruits[-1])

print(fruits[-2])
```

---

# Tuple Slicing

```python
numbers = (10,20,30,40,50)

print(numbers[1:4])

print(numbers[:3])

print(numbers[2:])
```

---

# Tuple Immutability

Tuples cannot be modified after creation.

```python
numbers = (1,2,3)

# numbers[0]=10 ❌ Error
```

---

# Updating Tuple

Although tuples are immutable, we can create a new tuple.

```python
t = (1,2,3)

t = t + (4,5)

print(t)
```

---

# Deleting Tuple

```python
t = (10,20,30)

del t
```

---

# Looping Through Tuple

```python
colors = ("Red","Green","Blue")

for color in colors:
    print(color)
```

---

# Membership Operators

```python
fruits = ("Apple","Banana","Orange")

print("Apple" in fruits)

print("Mango" not in fruits)
```

---

# Tuple Methods

## count()

Returns number of occurrences.

```python
numbers = (1,2,2,3,2)

print(numbers.count(2))
```

---

## index()

Returns first occurrence index.

```python
numbers = (10,20,30)

print(numbers.index(20))
```

---

# Packing

```python
student = ("Satyam",22,"India")
```

---

# Unpacking

```python
name, age, country = student

print(name)

print(age)

print(country)
```

---

# Nested Tuple

```python
data = (
    ("Satyam",22),
    ("Rahul",21),
    ("Aman",23)
)

print(data[0][0])
```

---

# Built-in Functions

```python
numbers = (10,20,30,40)

print(len(numbers))

print(max(numbers))

print(min(numbers))

print(sum(numbers))
```

---

# Tuple vs List

| Tuple | List |
|--------|------|
| Immutable | Mutable |
| Faster | Slower |
| Uses () | Uses [] |
| Less Memory | More Memory |
| Fixed Data | Frequently Changing Data |

---

# Advantages of Tuple

- Faster execution
- Less memory usage
- Data safety (immutable)
- Can be used as dictionary keys
- Good for fixed collections

---

# Disadvantages of Tuple

- Cannot modify elements
- Cannot append items
- Cannot remove items
- Less flexible than lists

---

# Summary

✔ Tuple

✔ Immutable

✔ Ordered

✔ Indexing

✔ Slicing

✔ Methods

✔ Packing

✔ Unpacking

✔ Nested Tuple

✔ Built-in Functions

✔ Tuple vs List

---

# Practice Questions

1. Create a tuple of five numbers.
2. Access the last element using negative indexing.
3. Count the occurrence of an element.
4. Find the index of an element.
5. Iterate through a tuple.
6. Demonstrate tuple packing and unpacking.
7. Create a nested tuple.
8. Find the maximum and minimum values in a tuple.
9. Explain why tuples are immutable.
10. Differentiate between tuple and list.

---

# Interview Questions

1. What is a tuple in Python?
2. Why are tuples immutable?
3. Difference between tuple and list?
4. What is tuple packing?
5. What is tuple unpacking?
6. Explain tuple slicing.
7. What are tuple methods?
8. Can a tuple contain mutable objects?
9. Why are tuples faster than lists?
10. When should we use tuples instead of lists?

---

🎉 Day 08 Completed Successfully 🚀