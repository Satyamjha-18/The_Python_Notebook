# Day 15 - Functional Programming

## 1. Functional Programming

Functional Programming is a programming paradigm where functions are used as the main building blocks of a program.

Python supports Functional Programming concepts such as:

- First-Class Functions
- Higher-Order Functions
- Lambda Functions
- map()
- filter()
- reduce()
- sorted()
- zip()
- any()
- all()
- List Comprehension
- Dictionary Comprehension

> Lambda Function Functional Programming ka ek part hai. Functional Programming sirf Lambda Function nahi hai.

---

## 2. First-Class Functions

Python me functions ko objects ki tarah treat kiya jata hai.

Function ko:
- Variable me store kar sakte hain
- Argument ke roop me pass kar sakte hain
- Return kar sakte hain

Example:

    def greet():
        return "Hello Python"

    message = greet

    print(message())

Output:

    Hello Python

---

## 3. Passing Function as an Argument

Ek function ko doosre function ke argument ke roop me pass kar sakte hain.

Example:

    def square(x):
        return x * x

    def calculate(func, value):
        return func(value)

    print(calculate(square, 5))

Output:

    25

---

## 4. Returning a Function

Ek function doosre function ko return kar sakta hai.

Example:

    def outer():

        def inner():
            print("Hello from inner function")

        return inner

    function = outer()
    function()

Output:

    Hello from inner function

---

## 5. Higher-Order Function

A Higher-Order Function is a function that:

1. Takes another function as an argument
2. OR returns another function

Example:

    def apply_operation(func, a, b):
        return func(a, b)

    add = lambda x, y: x + y

    print(apply_operation(add, 10, 20))

Output:

    30

---

# Lambda Function

## 6. What is Lambda Function?

Lambda function ek small anonymous function hota hai.

Iska koi normal function name nahi hota.

Syntax:

    lambda arguments: expression

Example:

    square = lambda x: x * x

    print(square(5))

Output:

    25

---

## 7. Lambda with Multiple Arguments

Example:

    add = lambda a, b: a + b

    print(add(10, 20))

Output:

    30

Another Example:

    maximum = lambda a, b: a if a > b else b

    print(maximum(10, 20))

Output:

    20

---

# map()

## 8. What is map()?

map() function iterable ke har element par given function apply karta hai.

Syntax:

    map(function, iterable)

Example:

    numbers = [1, 2, 3, 4, 5]

    result = map(lambda x: x * 2, numbers)

    print(list(result))

Output:

    [2, 4, 6, 8, 10]

---

## 9. map() with Normal Function

    def square(x):
        return x * x

    numbers = [1, 2, 3, 4]

    result = map(square, numbers)

    print(list(result))

Output:

    [1, 4, 9, 16]

---

## 10. map() with Multiple Lists

    a = [1, 2, 3]
    b = [4, 5, 6]

    result = map(lambda x, y: x + y, a, b)

    print(list(result))

Output:

    [5, 7, 9]

---

# filter()

## 11. What is filter()?

filter() function condition ke basis par elements ko select karta hai.

Syntax:

    filter(function, iterable)

Example:

    numbers = [1, 2, 3, 4, 5, 6]

    result = filter(lambda x: x % 2 == 0, numbers)

    print(list(result))

Output:

    [2, 4, 6]

---

## 12. Filter Positive Numbers

    numbers = [-5, 2, -1, 8, -3, 10]

    result = filter(lambda x: x > 0, numbers)

    print(list(result))

Output:

    [2, 8, 10]

---

## 13. Filter Numbers Greater Than 10

    numbers = [5, 12, 8, 20, 3, 15]

    result = filter(lambda x: x > 10, numbers)

    print(list(result))

Output:

    [12, 20, 15]

---

# reduce()

## 14. What is reduce()?

reduce() function multiple values ko repeatedly process karke ek single result produce karta hai.

reduce() ko functools module se import karna padta hai.

Example:

    from functools import reduce

    numbers = [1, 2, 3, 4, 5]

    result = reduce(lambda x, y: x + y, numbers)

    print(result)

Output:

    15

---

## 15. Product using reduce()

    from functools import reduce

    numbers = [1, 2, 3, 4, 5]

    result = reduce(lambda x, y: x * y, numbers)

    print(result)

Output:

    120

---

## 16. Maximum using reduce()

    from functools import reduce

    numbers = [10, 25, 5, 40, 15]

    maximum = reduce(lambda x, y: x if x > y else y, numbers)

    print(maximum)

Output:

    40

---

# sorted()

## 17. sorted() with Lambda

sorted() ka use data ko sort karne ke liye hota hai.

Lambda ko key ke saath use kar sakte hain.

    students = [
        ("Aman", 80),
        ("Rahul", 95),
        ("Satyam", 88)
    ]

    result = sorted(students, key=lambda x: x[1])

    print(result)

Output:

    [('Aman', 80), ('Satyam', 88), ('Rahul', 95)]

---

## 18. Sorting in Descending Order

    students = [
        ("Aman", 80),
        ("Rahul", 95),
        ("Satyam", 88)
    ]

    result = sorted(
        students,
        key=lambda x: x[1],
        reverse=True
    )

    print(result)

---

# zip()

## 19. What is zip()?

zip() multiple iterables ke corresponding elements ko combine karta hai.

Example:

    names = ["Aman", "Rahul", "Satyam"]
    marks = [80, 90, 85]

    result = zip(names, marks)

    print(list(result))

Output:

    [('Aman', 80), ('Rahul', 90), ('Satyam', 85)]

---

## 20. Creating Dictionary using zip()

    names = ["Aman", "Rahul", "Satyam"]
    marks = [80, 90, 85]

    students = dict(zip(names, marks))

    print(students)

Output:

    {'Aman': 80, 'Rahul': 90, 'Satyam': 85}

---

# any()

## 21. What is any()?

any() True return karta hai agar at least one condition True ho.

Example:

    numbers = [1, 3, 5, 8]

    result = any(x % 2 == 0 for x in numbers)

    print(result)

Output:

    True

Because 8 is even.

---

# all()

## 22. What is all()?

all() True return karta hai jab saari conditions True ho.

Example:

    numbers = [2, 4, 6, 8]

    result = all(x % 2 == 0 for x in numbers)

    print(result)

Output:

    True

---

## 23. Difference between any() and all()

any():

- At least one condition True honi chahiye.
- Ek True value enough hai.

all():

- Sabhi conditions True honi chahiye.
- Ek bhi False hua to result False hoga.

Example:

    numbers = [2, 4, 6, 8]

    print(any(x > 5 for x in numbers))
    print(all(x > 1 for x in numbers))

Output:

    True
    True

---

# List Comprehension

## 24. What is List Comprehension?

List comprehension short and readable way hai list create karne ka.

Normal method:

    numbers = []

    for i in range(1, 6):
        numbers.append(i * 2)

    print(numbers)

List comprehension:

    numbers = [i * 2 for i in range(1, 6)]

    print(numbers)

Output:

    [2, 4, 6, 8, 10]

---

## 25. List Comprehension with Condition

    numbers = [1, 2, 3, 4, 5, 6]

    even = [x for x in numbers if x % 2 == 0]

    print(even)

Output:

    [2, 4, 6]

---

# Dictionary Comprehension

## 26. What is Dictionary Comprehension?

Dictionary comprehension short way hai dictionary create karne ka.

Example:

    numbers = [1, 2, 3, 4]

    squares = {x: x * x for x in numbers}

    print(squares)

Output:

    {1: 1, 2: 4, 3: 9, 4: 16}

---

## 27. Dictionary Comprehension with Condition

    numbers = [1, 2, 3, 4, 5, 6]

    even_squares = {
        x: x * x
        for x in numbers
        if x % 2 == 0
    }

    print(even_squares)

Output:

    {2: 4, 4: 16, 6: 36}

---

# Practical Examples

## 28. Convert Names to Uppercase

    names = ["aman", "rahul", "satyam"]

    result = list(map(str.upper, names))

    print(result)

Output:

    ['AMAN', 'RAHUL', 'SATYAM']

---

## 29. Find Even Numbers

    numbers = [10, 15, 20, 25, 30]

    even = list(filter(lambda x: x % 2 == 0, numbers))

    print(even)

Output:

    [10, 20, 30]

---

## 30. Find Sum using reduce()

    from functools import reduce

    numbers = [10, 20, 30, 40]

    total = reduce(lambda x, y: x + y, numbers)

    print(total)

Output:

    100

---

## 31. Student Data Processing

    students = [
        ("Aman", 75),
        ("Rahul", 90),
        ("Satyam", 85),
        ("Vikas", 60)
    ]

    top_students = list(
        filter(lambda x: x[1] >= 80, students)
    )

    print(top_students)

Output:

    [('Rahul', 90), ('Satyam', 85)]

---

# Functional Programming Quick Revision

| Concept | Purpose |
|---|---|
| First-Class Function | Function ko object ki tarah use karna |
| Higher-Order Function | Function ko argument/return ke roop me use karna |
| lambda | Anonymous function |
| map() | Har element ko transform karna |
| filter() | Condition ke basis par filter karna |
| reduce() | Multiple values ko single result me reduce karna |
| sorted() | Data ko sort karna |
| zip() | Multiple iterables ko combine karna |
| any() | At least one True check karna |
| all() | All conditions True check karna |
| List Comprehension | Short way to create list |
| Dictionary Comprehension | Short way to create dictionary |

---

# Advantages of Functional Programming

- Code short and readable hota hai.
- Functions reusable hote hain.
- Data processing easy hoti hai.
- `map()`, `filter()` aur `reduce()` useful data-processing tools hain.
- Python Data Science aur Data Analytics me frequently used hai.
- Complex operations ko small functions me divide kar sakte hain.

---

# Practice Questions

1. Create a lambda function to find square of a number.
2. Create a lambda function to add two numbers.
3. Find maximum of two numbers using lambda.
4. Use map() to double all numbers.
5. Use map() to find squares.
6. Use filter() to find even numbers.
7. Use filter() to find positive numbers.
8. Use filter() to find numbers greater than 50.
9. Use reduce() to find sum.
10. Use reduce() to find product.
11. Find maximum using reduce().
12. Sort students according to marks.
13. Sort students in descending order.
14. Combine names and marks using zip().
15. Create dictionary using zip().
16. Check whether a list contains an even number using any().
17. Check whether all numbers are positive using all().
18. Create a list using list comprehension.
19. Create a dictionary using dictionary comprehension.
20. Create a program using map(), filter() and reduce().

---

# Interview Questions

1. What is Functional Programming?
2. Is Lambda Function the same as Functional Programming?
3. What are First-Class Functions?
4. What is a Higher-Order Function?
5. What is a Lambda Function?
6. What is the use of map()?
7. What is the difference between map() and filter()?
8. What is the use of reduce()?
9. From which module is reduce() imported?
10. What is the use of zip()?
11. What is the difference between any() and all()?
12. What is List Comprehension?
13. What is Dictionary Comprehension?
14. How can lambda be used with sorted()?
15. Why is Functional Programming useful in Python?

---

# Summary

Functional Programming is a programming paradigm that uses functions to process data.

Important concepts:

- First-Class Functions
- Higher-Order Functions
- Lambda Functions
- map()
- filter()
- reduce()
- sorted()
- zip()
- any()
- all()
- List Comprehension
- Dictionary Comprehension

Quick Revision:

lambda → Small anonymous function

map() → Transform elements

filter() → Select elements based on condition

reduce() → Reduce multiple values into one result

sorted() → Sort data

zip() → Combine iterables

any() → At least one condition True

all() → All conditions True

## Day 15 - Functional Programming Completed 🚀