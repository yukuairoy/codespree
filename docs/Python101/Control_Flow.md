---
comments: true
---

# Control Flow

## Conditionals
### `if-else`
```python
temperature = 30
if temperature > 25:
    print("It's hot!")
```

### `if-elif-else`
```python
if temperature > 25:
    print("It's hot!")
elif temperature > 15:
    print("It's warm.")
else:
    print("It's cold.")
```

### Ternary Operator
```python
status = "Adult" if age >= 18 else "Minor"
```

---
## Loops

### `for`-loop
The `for` loop is used to iterate over a sequence:

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
# Output:
# apple
# banana
# cherry
```

### `enumerate`
The `enumerate()` function gives both the index and the corresponding element:

```python
fruits = ["apple", "banana", "cherry"]
for index, fruit in enumerate(fruits):
    print(f"{index}: {fruit}")
# Output:
# 0: apple
# 1: banana
# 2: cherry
```

### `range`
The `range()` function generates a sequence of numbers:

```python
range(start, stop, step)
```
- `start`: Starting value (default is `0`).
- `stop`: End of the sequence (exclusive).
- `step`: Increment or decrement (default is `1`).

#### Basic Range
```python
for i in range(5):
    print(i)
# Output: 0, 1, 2, 3, 4
```

#### Custom Start and Stop
```python
for i in range(2, 6):
    print(i)
# Output: 2, 3, 4, 5
```

#### Step Values
```python
for i in range(0, 10, 2):
    print(i)
# Output: 0, 2, 4, 6, 8
```

#### Reverse Range
```python
for i in range(10, 0, -2):
    print(i)
# Output: 10, 8, 6, 4, 2
```

---
## Exception Handling

### Basic Exception Handling

[`try`](https://docs.python.org/3/reference/compound_stmts.html#the-try-statement) blocks allow you to test a block of code for errors, while the [`except`](https://docs.python.org/3/reference/compound_stmts.html#except-clause) block lets you handle the error gracefully without stopping the program.

```python
try:
    x = 1 / 0
except ZeroDivisionError:
    print("Can't divide by zero!")
```

### Multiple Exception Types
You can catch multiple exceptions to handle different error types distinctly:

```python
try:
  # Code that might raise different exceptions
except ValueError:
  print("Value error occurred.")
except ZeroDivisionError:
  print("Division by zero.")
```

### [`finally`](https://docs.python.org/3/reference/compound_stmts.html#finally-clause) Block
`finally` ensures that a block of code is executed, regardless of an exception being thrown or not. It's often used for cleaning up resources.

```python
try:
  # Risky code
except Exception as e:
  print(f"An error occurred: {e}")
finally:
  print("This block executes no matter what.")
```

---
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T416OJAV)