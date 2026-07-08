# 📅 Day 03 - Operators in Python

# What is an Operator?

An operator is a special symbol used to perform operations on variables and values.

Example

```python
a = 10
b = 5

print(a + b)
```

Output

```
15
```

---

# Types of Operators

Python provides the following operators:

- Arithmetic Operators
- Assignment Operators
- Comparison Operators
- Logical Operators
- Identity Operators
- Membership Operators
- Bitwise Operators

---

# 1. Arithmetic Operators

Used to perform mathematical calculations.

| Operator | Meaning        | Example |
|----------|  ---------     |---------|
|    +     | Addition       |  a+b    |
|    -     | Subtraction    |  a-b    |
|    *     | Multiplication |  a*b    |
|    /     | Division       |  a/b    |
|    //    | Floor Division |  a//b   |
|    %     | Modulus        |  a%b    |
|   **     | Exponent       |  a**b   |

Example

a = 20
b = 6

print(a+b)
print(a-b)
print(a*b)
print(a/b)
print(a//b)
print(a%b)
print(a**2)

---

# 2. Assignment Operators

Used to assign values.

| Operator | Example |
|----------|----------|
|    =     | x=5      |
|   +=     | x+=2     |
|   -=     | x-=2     |
|   *=     | x*=2     |
|   /=     | x/=2     |
|   //=    | x//=2    |
|   %=     | x%=2     |
|   **=    | x**=2    |


# 3. Comparison Operators

Return True or False.

| Operator | Meaning             |
|----------|---------------------|
|   ==     |  Equal              |
|   !=     |  Not Equal          |
|   >      |  Greater Than       |
|   <      |  Less Than          |
|   >=     |  Greater Than Equal |
|   <=     |  Less Than Equal    |

Example

a = 10
b = 20

print(a==b)
print(a!=b)
print(a>b)
print(a<b)


# 4. Logical Operators

Used to combine conditions.

| Operator |  Meaning             |
|----------| ---------------------|
|  and     | Both conditions True |
|  or      | At least one True    |
|  not     | Reverse result       |

Example

```python
age = 20

print(age>18 and age<30)
print(age>18 or age>50)
print(not(age>18))
```

---

# 5. Identity Operators

Used to compare object identity.

| Operator | Meaning          |
|----------|------------------|
| is       | Same Object      |
| is not   | Different Object |

Example

a = [1,2]
b = a

print(a is b)
print(a is not b)



# 6. Membership Operators

Check whether a value exists.

| Operator |  Meaning      |
|----------|---------------|
| in       | Exists        |
| not in   | Doesn't Exist |

Example

fruits = ["Apple","Banana","Mango"]

print("Apple" in fruits)
print("Orange" not in fruits)
```

---

# 7. Bitwise Operators

Used on binary numbers.

| Operator | Meaning     |
|----------|------------ |
|    &     | AND         |
|   \|     | OR          |
|   ^      | XOR         |
|   ~      | NOT         |
|   <<     | Left Shift  |
|   >>     | Right Shift |

---

# Operator Precedence

Highest to Lowest

1. ()
2. **
3. *, /, //, %
4. +, -
5. Comparison
6. not
7. and
8. or

Example

print(10+5*2)
print((10+5)*2)

---

# Interview Questions

### What is an operator?

An operator is a symbol used to perform operations on operands.

---

### Difference between / and // ?

|       /       |       //        |
|---------------|-----------------|
| Returns Float | Returns Integer |

---

### Difference between == and is ?

== compares values.

is compares memory locations.

---

### Difference between and & or ?

and returns True only when both conditions are True.

or returns True when at least one condition is True.

---

# Summary

✔ Arithmetic Operators

✔ Assignment Operators

✔ Comparison Operators

✔ Logical Operators

✔ Identity Operators

✔ Membership Operators

✔ Bitwise Operators

✔ Operator Precedence

✔ Interview Questions

---

🎉 Day 03 Completed Successfully 🚀