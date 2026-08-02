# 📘 Day 10 - Set in Python

# What is a Set?

A Set is an unordered and mutable collection of unique elements.

- Stores only unique values
- Does not allow duplicates
- Mutable
- Unordered
- Faster searching than lists

Example:

```python
numbers = {10,20,30,40}
```

---

# Characteristics of Set

✔ Unique Elements

✔ Mutable

✔ Unordered

✔ No Duplicate Values

✔ Supports Mathematical Operations

---

# Creating a Set

```python
fruits = {"Apple","Banana","Mango"}
```

---

# Empty Set

```python
s = set()
```

> Don't use `{}` because it creates a dictionary.

---

# Accessing Elements

```python
fruits = {"Apple","Banana","Mango"}

for item in fruits:
    print(item)
```

---

# Membership Operator

```python
print("Apple" in fruits)
print("Orange" in fruits)
```

---

# Adding Elements

```python
fruits.add("Orange")
```

---

# Updating a Set

```python
fruits.update(["Grapes","Kiwi"])
```

---

# Removing Elements

## remove()

```python
fruits.remove("Banana")
```

Raises KeyError if element doesn't exist.

---

## discard()

```python
fruits.discard("Banana")
```

No error if element doesn't exist.

---

## pop()

```python
fruits.pop()
```

Removes a random element.

---

## clear()

```python
fruits.clear()
```

Removes all elements.

---

# Set Operations

## Union

```python
A = {1,2,3}
B = {3,4,5}

print(A.union(B))
```

---

## Intersection

```python
print(A.intersection(B))
```

---

## Difference

```python
print(A.difference(B))
```

---

## Symmetric Difference

```python
print(A.symmetric_difference(B))
```

---

# Set Methods

- add()
- update()
- remove()
- discard()
- pop()
- clear()
- copy()
- union()
- intersection()
- difference()
- symmetric_difference()
- issubset()
- issuperset()
- isdisjoint()

---

# Frozen Set

A Frozen Set is an immutable version of a set.

```python
fs = frozenset([1,2,3,4])
```

---

# Set Comprehension

```python
square = {x*x for x in range(1,6)}

print(square)
```

---

# Built-in Functions

```python
numbers = {10,20,30}

print(len(numbers))
print(max(numbers))
print(min(numbers))
print(sum(numbers))
```

---

# Remove Duplicate Values

```python
numbers = [10,20,30,20,10]

unique = list(set(numbers))

print(unique)
```

---

# Set vs List

| Set | List |
|------|------|
| Unique values | Duplicate values allowed |
| Unordered | Ordered |
| Uses {} | Uses [] |
| Fast lookup | Slower lookup |

---

# Advantages

- Removes duplicates automatically
- Fast searching
- Supports mathematical operations
- Efficient membership testing

---

# Disadvantages

- No indexing
- Unordered
- Cannot store mutable objects like lists

---

# Summary

✔ Set

✔ Unique Elements

✔ Mutable

✔ add()

✔ remove()

✔ discard()

✔ pop()

✔ Union

✔ Intersection

✔ Difference

✔ Symmetric Difference

✔ Frozen Set

✔ Set Comprehension

---

# Practice Questions

1. Create a set.
2. Add a new element.
3. Remove an element.
4. Remove duplicates from a list.
5. Find union of two sets.
6. Find intersection.
7. Find difference.
8. Find symmetric difference.
9. Check subset.
10. Create a frozen set.

---

# Interview Questions

1. What is a Set?
2. Difference between Set and List?
3. Difference between remove() and discard()?
4. What is Frozen Set?
5. Difference between union() and intersection()?
6. What is symmetric_difference()?
7. Why doesn't Set allow duplicates?
8. Can a Set contain a List?
9. Difference between pop() and remove()?
10. When should you use a Set?

---

🎉 Day 10 Completed Successfully 🚀