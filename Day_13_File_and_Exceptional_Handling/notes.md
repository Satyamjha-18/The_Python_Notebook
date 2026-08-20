# Day 13 - Exception Handling

## 1. What is Exception Handling?

Exception Handling is used to handle runtime errors in a Python program without stopping the complete program.

Example:

num = 10
result = num / 0

This gives ZeroDivisionError.

## 2. Why Exception Handling?

- Prevents program from crashing
- Handles runtime errors
- Makes programs more reliable
- Provides user-friendly error messages

## 3. try Block

The try block contains code that may produce an error.

```python
try:
    result = 10 / 0
4. except Block

The except block is used to handle the exception.


13. Common Python Exceptions
| Exception           | When it        Occurs                 |
| ------------------- | ------------------------------ |
| `ValueError`        | Invalid value                  |
| `TypeError`         | Incompatible data types        |
| `ZeroDivisionError` | Division by zero               |
| `FileNotFoundError` | File doesn't exist             |
| `IndexError`        | Invalid index                  |
| `KeyError`          | Dictionary key doesn't exist   |
| `NameError`         | Variable is not defined        |
| `AttributeError`    | Attribute/method doesn't exist |
| `PermissionError`   | Access permission denied       |
