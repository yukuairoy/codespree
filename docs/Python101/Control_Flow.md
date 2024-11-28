# Control Flow

## Conditional Statements
### `if` Statement

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

## Loops

### The `for` Loop
The `for` loop is used to iterate over a sequence.

**Example**:
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
# Output:
# apple
# banana
# cherry
```

### Using `enumerate`
The `enumerate()` function gives both the index and the corresponding element.

**Example**:
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

**Examples**

**Basic Range**:
```python
for i in range(5):
    print(i)
# Output: 0, 1, 2, 3, 4
```

**Custom Start and Stop**:
```python
for i in range(2, 6):
    print(i)
# Output: 2, 3, 4, 5
```

**Step Values**:
```python
for i in range(0, 10, 2):
    print(i)
# Output: 0, 2, 4, 6, 8
```

**Reverse Range**:
```python
for i in range(10, 0, -2):
    print(i)
# Output: 10, 8, 6, 4, 2
```

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T416OJAV)
