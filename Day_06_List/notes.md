# 📅 Day 06 - Lists in Python

# What is a List?

A List is an ordered, mutable (changeable) collection that can store multiple items of different data types.

Lists are created using square brackets [].

Example

```python
fruits = ["Apple", "Banana", "Mango"]
```

---

# Features of Lists

- Ordered
- Mutable
- Allows Duplicate Values
- Can Store Multiple Data Types
- Supports Indexing and Slicing

---

# Creating Lists

```python
numbers = [10,20,30]

names = ["Aman","Rahul","Satyam"]

mixed = [10,"Python",True,5.5]
```

---

# List Indexing

```python
fruits = ["Apple","Banana","Mango"]

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

# List Slicing

```python
numbers = [10,20,30,40,50]

print(numbers[1:4])

print(numbers[:3])

print(numbers[::2])
```

---

# Updating List

```python
fruits[1] = "Orange"

print(fruits)
```

---

# Adding Elements

append()

```python
fruits.append("Grapes")
```

insert()

```python
fruits.insert(1,"Kiwi")
```

extend()

```python
fruits.extend(["Papaya","Cherry"])
```

---

# Removing Elements

remove()

```python
fruits.remove("Apple")
```

pop()

```python
fruits.pop()
```

clear()

```python
fruits.clear()
```

del

```python
del fruits[0]
```

---

# Common List Methods

| Method | Description |
|---------|-------------|
| append() | Add at end |
| insert() | Insert at index |
| extend() | Add multiple items |
| remove() | Remove by value |
| pop() | Remove by index |
| clear() | Remove all elements |
| index() | Find index |
| count() | Count occurrences |
| sort() | Sort list |
| reverse() | Reverse list |
| copy() | Copy list |

---

# Loop Through List

```python
for item in fruits:
    print(item)
```

---

# Nested Lists

```python
matrix = [[1,2],[3,4],[5,6]]
```

---

# List Comprehension

```python
squares = [x*x for x in range(1,6)]

print(squares)
```

---

# Copy List

```python
new_list = fruits.copy()
```

---

# Sort List

```python
numbers.sort()

numbers.sort(reverse=True)
```

---

# Difference between append() and extend()

append() adds one item.

extend() adds multiple items.

---

# Summary

✔ Creating Lists

✔ Indexing

✔ Slicing

✔ Updating

✔ Adding Elements

✔ Removing Elements

✔ List Methods

✔ Nested Lists

✔ List Comprehension

✔ Sorting

---

🎉 Day 06 Completed Successfully 🚀