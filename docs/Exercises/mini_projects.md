---
comments: true
---

# Mini-Projects

This document contains a collection of mini-projects to enhance your programming skills and understanding of core concepts. These projects are perfect for:

* Gaining hands-on experience through real-world simulations.
* Building confidence and sharpening problem-solving abilities.
* Creating a portfolio to showcase your coding proficiency.
* Preparing for technical interviews by tackling practical problems.

---

## Problem 1: Password Strength Checker

Create a function that evaluates password strength based on the following criteria:

**Weak Password (Return "weak"):**

* Length less than 8 characters, OR
* Contains only letters, OR
* Contains only numbers

**Medium Password (Return "medium"):**

* Length 8-11 characters, AND
* Contains at least one letter and one number

**Strong Password (Return "strong"):**

* Length 12 or more characters, AND
* Contains at least one uppercase letter
* Contains at least one lowercase letter
* Contains at least one number
* Contains at least one special character from @#$%^&\*!

**Examples:**
```
Input: "password123"
Output: "medium"

Input: "abc12"
Output: "weak"

Input: "MySecurePass123!"
Output: "strong"

Input: "11111111"
Output: "weak"

Input: "Pass123!@"
Output: "medium"
```

---

## Problem 2: Parking System

Design a parking system for a parking lot with three types of parking spaces: **big**, **medium**, and **small**. Each type has a fixed number of parking slots available.

Implement the `ParkingSystem` class with the following methods:

* `__init__(self, big: int, medium: int, small: int)`: Initializes an object of the `ParkingSystem` class. The constructor accepts three integers representing the number of available parking slots for **big**, **medium**, and **small** cars, respectively.
* `addCar(self, car_type: str) -> bool`: Checks if there is an available parking slot for the car of the given `car_type`. If there is an available slot for the given car type, the car is parked, the available slots for that type are reduced by 1, and the method returns `True`. If no slots are available for the car type, the method returns `False`.

**Example**:

```python
# Initialize the parking system with:
# 2 slots for big cars, 1 slot for medium cars, and 0 slots for small cars.
ps = ParkingSystem(2, 1, 0)

# Try to park cars of different types.
print(ps.addCar("big"))     # Output: True (1 slot for big cars now remaining)
print(ps.addCar("big"))     # Output: True (0 slots for big cars now remaining)
print(ps.addCar("medium"))  # Output: True (0 slots for medium cars now remaining)
print(ps.addCar("small"))   # Output: False (no slots available for small cars)
print(ps.addCar("medium"))  # Output: False (no slots available for medium cars)
print(ps.addCar("big"))     # Output: False (no slots available for big cars)
```

---

## Problem 3: Validate Credit Card

The [Luhn algorithm](https://en.wikipedia.org/wiki/Luhn_algorithm) is a checksum formula used to validate credit card numbers.

The checksum of `cc_no`, a credit card number represented as a string, is computed as follows:

1. Reverse the order of the digits in `cc_no` and name it `cc_no_reversed`.
2. Add up `cc_no_reversed[0]`, `cc_no_reversed[2]`, ... and every other even index digit to form the partial sum `s1`
3. Taking `cc_no_reversed[1]`, `cc_no_reversed[3]`, ... and every other odd index digit:

* Multiply each digit by 2. If doubling a digit results in a two digit number, add those digits together to produce a single digit number
* Sum the partial sums of the even digits to form `s2`

The checksum is `s1 + s2`. Luhn algorithm determines `cc_no` is valid when the checksum ends in zero.

**Example**

```
If the credit card number is 49927398716:

1. Reverse the digits: 61789372994
2. Sum the even index digits: s1 = 6 + 7 + 9 + 7 + 9 + 4 = 42
3. The odd index digits: 1, 8, 3, 2, 9
   * Multiply each of them by 2: 2, 16, 6, 4, 18
   * Sum the digits of each multiplication: 2, 7, 6, 4, 9
   * s2 = 2 + 7 + 6 + 4 + 9 = 28

The checksum is s1 + s2 = 70 which ends in zero. So, 49927398716 is valid.
```

Your task is to implement the Luhn algorithm.

---

## Problem 4: Guess the Number

Build a game where the player guesses a number randomly selected by the computer. The game should:

1. Pick a random number between 1 and 100.
2. Allow the player to make repeated guesses.
3. Provide feedback: "higher," "lower," or "correct."
4. Track and display the number of attempts.
5. Optionally, restart the game for another round after completion.

**Examples:**
```
Computer: "Guess a number between 1 and 100."
Player: 50
Computer: "Higher."
Player: 75
Computer: "Lower."
Player: 63
Computer: "Correct! You took 3 attempts."
```

---

## Problem 5: Hangman Game

Create a Hangman game where:

1. The computer randomly selects a word from a predefined list.
2. The player has 6 attempts to guess the word, letter by letter.
3. The game displays a hangman figure representing incorrect guesses.
4. Correctly guessed letters appear in their positions; underscores `_` represent unguessed letters.
5. The game ends when the player either guesses the word or uses all attempts.

**Examples:**
```
Word: "python"
Player guesses: "a", "e", "o"
Display: "_ _ _ _ o _"
Remaining attempts: 4

Player guesses: "p", "t", "h", "n"
Display: "p y t h o n"
Game Result: Player Wins!
```

---

## Problem 6: Tic-Tac-Toe

Build a two-player Tic-Tac-Toe game where:

1. A 3x3 grid represents the board.
2. Players take turns to place their marker (`X` or `O`) in an empty cell.
3. The game ends when one player gets 3 markers in a row, column, or diagonal, or when all cells are filled (tie).
4. A function checks for a win condition after every move.

**Examples:**
```
Initial board:
 1 | 2 | 3
---+---+---
 4 | 5 | 6
---+---+---
 7 | 8 | 9

Player 1 (X): Selects position 1
Updated board:
 X | 2 | 3
---+---+---
 4 | 5 | 6
---+---+---
 7 | 8 | 9

Player 2 (O): Selects position 5
Updated board:
 X | 2 | 3
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | 9

Player 1 (X): Selects position 3
Updated board:
 X | 2 | X
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | 9

Player 2 (O): Selects position 9
Updated board:
 X | 2 | X
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | O

Player 1 (X): Selects position 2
Updated board:
 X | X | X
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | O
Game Result: Player 1 Wins!
```

---

## Problem 7: Exponential Backoff

You are implementing an [exponential backoff](https://en.wikipedia.org/wiki/Exponential_backoff) mechanism commonly used in networking and distributed systems for retrying operations. The goal is to retry an operation multiple times with an exponentially increasing delay between attempts. If all retries fail, return a failure message.

Write a function `exponential_backoff` that takes the following parameters:

- `operation`: A callable function that performs the operation and may raise an exception on failure.
- `max_retries`: An integer representing the maximum number of retry attempts.

The function should:

1. Retry the `operation` up to `max_retries` times if it fails.
2. Use an exponential backoff delay: $2^{i-1}$ seconds for the $i^{th}$ retry (e.g., 1 second for the first retry, 2 seconds for the second retry, etc.).
3. Return the result of the `operation` if it succeeds within the allowed retries.
4. If all retries fail, raise an exception indicating that the operation failed after all attempts.

**Examples:**

**Example 1: Operation succeeds after retries**

```python
def unreliable_operation():
    import random
    if random.random() < 0.5:  # 50% chance of success
        return "Success"
    raise Exception("Operation failed")

print(exponential_backoff(unreliable_operation, max_retries=5))
```

Output (sample):

```
Attempt 1 failed. Retrying in 1 seconds...
Attempt 2 failed. Retrying in 2 seconds...
Attempt 3 succeeded: Success
```

**Example 2: Operation fails completely**

```python
def always_failing_operation():
    raise Exception("Operation failed")

print(exponential_backoff(always_failing_operation, max_retries=3))
```

Output:

```
Attempt 1 failed. Retrying in 1 seconds...
Attempt 2 failed. Retrying in 2 seconds...
Attempt 3 failed. Operation failed after 3 attempts.
```

**Hints**

- Use `time.sleep()` for delays between retries.
- Catch exceptions with `try-except` blocks during each retry.
- Compute the delay as \(2^{i-1}\) seconds for the \(i^{th}\) attempt.

---

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T416OJAV)