---
comments: true
---

# Python Basics

## Functions

### Basic Structure
```python
def greet(name):
    return f"Hello, {name}!"

greet("Alice")
```

### Default Arguments
```python
def greet(name="User"):
    print(f"Hello, {name}!")
```

### Functions as First-Class Citizens

In Python, functions are first-class citizens. This means you can use functions as variables, pass them as arguments to other functions, and return them from functions.

```python
def greet(name):
    return f"Hello, {name}!"

def caller(func, arg):
    return func(arg)

print(caller(greet, "Alice"))  # Output: Hello, Alice!
```

---
## Data Types

**Common Data Types**:

- `int` (e.g., `age = 25`)
- `float` (e.g., `height = 5.9`)
- `bool` (e.g., `is_student = True`)
- `str` (e.g., `name = "Alice"`)
- `list` (e.g., `nums = [3, 1, 4]`)
- `NoneType` (e.g., `status = None`)

**Example**:
```python
name = "Alice"
age = 25
print(name + " is " + str(age) + " years old.")
print(f"{name} is {age} years old.")
```

### Type Conversion
Python provides functions to convert data between types:
```python
num_str = "100"
num = int(num_str)
print(float(num))  # 100.0
```

---
## Logical Operators
- `and`: Returns `True` if both conditions are `True`.
- `or`: Returns `True` if at least one condition is `True`.
- `not`: Inverts a boolean value.

### Truthy and Falsey
```python
if []:  # An empty list is False
    print("This won't print.")
if [1, 2]:  # A non-empty list is True
    print("This will print.")
```

---
## `input()`
The `input()` function allows users to provide input to the program during runtime:

```python
name = input("What is your name? ")
print(f"Hello, {name}!")

age = int(input("Enter your age: "))
print(f"You will be {age + 1} next year!")
```

---
## File Handling

```python
# Writing to a file
with open("example.txt", "w") as file:
    file.write("Hello, Python!")

# Reading from a file
with open("example.txt", "r") as file:
    content = file.read()
    print(content)
```

---
## Common Python Errors
### SyntaxError
```python
print("Hello)  # Missing closing quotation
```

### TypeError
```python
"2" + 2  # Can't add string and integer
```

### NameError
```python
print(x)  # x is not defined
```
### IndexError
```python
['cat', 'dog', 'rabbit'][3] # IndexError: list index out of range
```

---
## Comments
### Single-Line Comments
```python
# This is a comment
print("Hello!")  # Another comment
```

### Multi-Line Comments
```python
'''
This is a multi-line comment.
Useful for longer explanations.
'''
print("Hello!")
```

---
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T416OJAV)