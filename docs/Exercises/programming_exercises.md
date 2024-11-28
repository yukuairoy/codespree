---
comments: true
---

# Programming Exercises

This document features simple programming exercises to sharpen your skills in foundational concepts like strings, numbers, lists, and algorithms. Ideal for:

* Learning a new programming language by implementing hands-on solutions.
* Refreshing skills in a language you haven’t used recently.
* Preparing for coding interviews as a stepping stone to platforms like [LeetCode](https://leetcode.com/) or [HackerRank](https://www.hackerrank.com/).
* Building confidence with approachable problems before tackling advanced ones.
* Improving problem-solving, debugging, and optimization skills.
* Practicing unit testing, a crucial skill for professional development.

---
## Problem 1: Vowel Counter

Write a program that counts the number of vowels in a given word. Vowels are `a`, `e`, `i`, `o`, `u` (case-insensitive).

**Examples**

```plaintext
Input: "hello"
Output: 2

Input: "education"
Output: 5

Input: "rhythm"
Output: 0
```

---
## Problem 2: Reverse a List

Write a function to reverse a list.

**Examples:**  
```plaintext
Input: [1, 2, 3, 4, 5]
Output: [5, 4, 3, 2, 1]

Input: [10, 20, 30]
Output: [30, 20, 10]
```

---
## Problem 3: Perfect Square

Check if a number is a [perfect square](https://en.wikipedia.org/wiki/Square_number). A perfect square is an integer that is the square of another integer.

**Examples**

```plaintext
Input: 16
Output: True

Input: 18
Output: False

Input: 1
Output: True
```

---
## Problem 4: Sum of Digits in a Number

Write a function to calculate the sum of digits in a given number.

**Examples:**
```plaintext
Input: 12345
Output: 15

Input: 9876
Output: 30
```

---
## Problem 5: [Sum of Digits](https://en.wikipedia.org/wiki/Digital_root)

Add all digits in a number until you get a single digit.

**Examples**
```plaintext
Input: 789
Output: 6 (7+8+9=24, 2+4=6)

Input: 1234
Output: 1 (1+2+3+4=10, 1+0=1)

Input: 5
Output: 5
```

---

## Problem 6: Second Largest

Find the second largest number in an array.

**Examples**
```plaintext
Input: [10, 5, 8, 12]
Output: 10

Input: [1, 2, 3, 4, 5]
Output: 4

Input: [5, 5, 5, 5]
Output: 5
```

---
## Problem 7: Array Rotation

Rotate an array by `k` positions to the right.

**Examples:**
```plaintext
Input: [1, 2, 3, 4], k=2
Output: [3, 4, 1, 2]

Input: [10, 20, 30, 40, 50], k=3
Output: [30, 40, 50, 10, 20]

Input: [1, 2, 3], k=0
Output: [1, 2, 3]
```

---

## Problem 8: Number Triangle

Print a triangle pattern of numbers where each row contains increasing numbers starting from 1.

**Examples:**
```plaintext
Input: n=3
Output:
1
1 2
1 2 3

Input: n=5
Output:
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

---
## Problem 9: Email Validator

Write a program that validates an email address based on the following rules:

1. Contains exactly one `@`.
2. The part before `@` contains only valid characters (letters, numbers, underscores, or dots).
3. The part after `@` is a valid domain (letters and periods).
4. The email contains no spaces.

**Examples:**
```plaintext
Input: "test.email@domain.com"
Output: Valid

Input: "invalid@@domain.com"
Output: Invalid

Input: "user name@domain.com"
Output: Invalid
```

---
## Problem 10: Phone Number Formatter

Write a program that formats a 10-digit phone number into the format `(XXX) XXX-XXXX`.

**Examples**  
```plaintext
Input: "1234567890"
Output: "(123) 456-7890"

Input: "9876543210"
Output: "(987) 654-3210"

Input: "(123)-456-7890"
Output: "(123) 456-7890"
```

---
## Problem 11: Find the Extra Character

Given two strings, `A` and `B`, where `A` has exactly one extra character compared to `B`, find that character.

**Examples:**  
```plaintext
Input: A = "atcb42c", B = "atb42c"
Output: "c"

Input: A = "abcd", B = "abc"
Output: "d"
```

---
## Problem 12: First Non-Repeating Character

Given a string, find the index of the first non-repeating character. Return `-1` if no such character exists.

**Examples:**  
```plaintext
Input: "lastlasp"
Output: 3

Input: "sophhpho"
Output: 0
```

---
## Problem 13: K-th Fibonacci Number

Find the `k-th` [Fibonacci number](https://en.wikipedia.org/wiki/Fibonacci_sequence).

**Examples:**  
```plaintext
Input: k = 5
Output: 5

Input: k = 10
Output: 55
```

---
## Problem 14: Add Two Numbers Represented as Strings

Write a function to add two numbers represented as strings. Return the sum as a string.

**Examples:**  
```plaintext
Input: num1 = "123", num2 = "456"
Output: "579"

Input: num1 = "999", num2 = "1"
Output: "1000"
```

---
## Problem 15: Product of Array Except Self

Given an array of integers, return a new array such that each element at index `i` is the product of all numbers in the original array except the one at `i`.

**Examples:**  
```plaintext
Input: [1, 2, 3, 4, 5]
Output:  [120, 60, 40, 30, 24]

Input: [3, 2, 1]
Output: [2, 3, 6]
```

---

## Problem 16: Largest Sum of Non-Adjacent Numbers

Given a list of integers, write a function that returns the largest sum of non-adjacent numbers. Numbers can be zero or negative.

**Examples:**  
```plaintext
Input: [2, 4, 6, 8]
Output: 12

Input: [5, 1, 1, 5]
Output: 10
```

---
## Problem 17: Implement [Power Function](https://en.wikipedia.org/wiki/Exponentiation)

Implement the function `pow(x, y)` to compute \(x^y\).

**Examples:**  
```plaintext
Input: x = 2, y = 3
Output: 8

Input: x = 5, y = -2
Output: 0.04
```

---
## Problem 18: [Combinations](https://en.wikipedia.org/wiki/Combination)

Write a function to compute the number of ways to choose `k` items from `n` items (combinations), denoted as \(C(n, k)\).

**Examples:**  
```plaintext
Input: n = 5, k = 2
Output: 10

Input: n = 6, k = 3
Output: 20
```

---
## Problem 19: Count Unique Characters in a String

Write a function that counts the number of unique characters in a string.

**Examples:**
```plaintext
Input: "programming"
Output: 8

Input: "hello"
Output: 4
```

---
## Problem 20: Check for [Palindrome](https://en.wikipedia.org/wiki/Palindrome)

Write a function to check if a given string is a palindrome.

**Examples:**
```plaintext
Input:  "madam"
Output: True

Input: "hello"
Output: False
```

---
## Problem 21: Check if Two Strings are [Anagrams](https://en.wikipedia.org/wiki/Anagram)

Write a function to check if two strings are anagrams of each other.

**Examples:**  
```plaintext
Input: "listen", "silent"
Output: True

Input: "apple", "pale"
Output: False
```

---
## Problem 22: Check If a Number is [Prime](https://en.wikipedia.org/wiki/Prime_number)

Write a function to determine if a given number is prime.

**Examples:**  

```plaintext
Input: 13
Output: True

Input: 10
Output: False
```

---
## Problem 23: Find the Missing Number

Given an array containing `n` distinct numbers taken from the range `[0, n]`, find the missing number.

**Examples:**

```plaintext
Input: [3, 0, 1]
Output: 2

Input: [2, 3, 1, 4, 5]
Output: 0
```

---
## Problem 24: String Reversal

Write a function to reverse a string.

**Example:**  
```plaintext
Input: "hello"
Output: "olleh"
```

---
## Problem 25: Reverse Words

Given a sentence, reverse the order of words.

**Examples**

```plaintext
Input: "The quick brown fox"
Output: "fox brown quick The"

Input: "Hello world!"
Output: "world! Hello"
```

---
## Problem 26: Convert a List to a Single String

Write a function that takes a list of strings and concatenates them into a single string, separated by commas.

**Example:**  

```plaintext
Input: ["apple", "banana", "cherry"]
Output: "apple,banana,cherry"
```

---
## Problem 27: Convert Temperature

Write a function to [convert temperature between Celsius and Fahrenheit](https://en.wikipedia.org/wiki/Fahrenheit#Conversion_(specific_temperature_point)).

**Examples:**  
```plaintext
Input: temp = 100, scale = "C"  # Convert from Celsius to Fahrenheit
Output: 212

Input: temp = 32, scale = "F"  # Convert from Fahrenheit to Celsius
Output: 0
```

---
## Problem 28: Diamond Pattern

Print a diamond pattern using asterisks (`*`).

**Examples**  
```plaintext
Input: 3
Output:
  *
 ***
*****
 ***
  *

Input: 5
Output:
    *
   ***
  *****
 *******
*********
 *******
  *****
   ***
    *
```

---
## Problem 29: Check if a String is a [Pangram](https://en.wikipedia.org/wiki/Pangram)

Write a function to check if a given string is a pangram (contains every letter of the alphabet at least once).

**Example:**  
 
```plaintext
Input: "The quick brown fox jumps over the lazy dog"
Output: True
```

---
## Problem 30: Count Words in a String

Write a program to count the number of words in a given string.

**Example:**  
 
```plaintext
Input: "This is a test string."
Output: 5
```

---

## Problem 31: Calculate [Factorial](https://en.wikipedia.org/wiki/Factorial)

Write a function to calculate the factorial of a given number using recursion.

**Example:**

```plaintext
Input: 5
Output: 120
```

---
## Problem 32: Compute [Double Factorial](https://en.wikipedia.org/wiki/Double_factorial)

Write a function that computes the double factorial of a given non-negative integer `n`.  
The double factorial of `n`, denoted as `n!!`, is defined as the product of all integers from 1 to `n` that have the same parity (odd or even) as `n`.  

**Examples:**
```plaintext
Input: n = 8
Output: 384
Explanation: 8!! = 8 * 6 * 4 * 2 = 384

Input: n = 7
Output: 105
Explanation: 7!! = 7 * 5 * 3 * 1 = 105
```

---
## Problem 33: Title Case

Convert a sentence to [title case](https://en.wikipedia.org/wiki/Title_case) where each word starts with a capital letter, and the rest of the letters in the word are lowercase.

**Examples**
```plaintext
Input: "hello world"
Output: "Hello World"

Input: "this is a TEST"
Output: "This Is A Test"

Input: "programming is fun"
Output: "Programming Is Fun"
```

---
## Problem 34: Check [Perfect Number](https://en.wikipedia.org/wiki/Perfect_number)

Write a function to check if a number is a perfect number. A perfect number is a positive integer equal to the sum of its proper divisors (excluding itself).

**Example:**
```plaintext
Input: 6
Output: True
```

---

## Problem 35: Count Prime Factors of a Number

Write a function to count the number of prime factors of a given positive integer. A prime factor is a prime number that divides the given number exactly.

**Example:**  
```plaintext
Input: 60
Output: 3
Explanation: The prime factors of 60 are 2, 3, and 5.

Input: 100
Output: 2
Explanation: The prime factors of 100 are 2 and 5.

Input: 37
Output: 1
Explanation: The prime factor of 37 is 37 itself (it's a prime number).

Input: 1
Output: 0
Explanation: 1 has no prime factors.

Input: 84
Output: 3
Explanation: The prime factors of 84 are 2, 3, and 7.
```

---
## Problem 36: Check [Derangement](https://en.wikipedia.org/wiki/Derangement)

Write a function to check if one permutation of a string is a derangement of another. A derangement means no character appears in its original position.

**Examples:**  
```plaintext
Input: s1 = "abc", s2 = "cab"
Output: True

Input: s1 = "abc", s2 = "bac"
Output: False
```

---
## Problem 37: Check [Narcissistic Number](https://en.wikipedia.org/wiki/Narcissistic_number)

Write a function to check if a number is a narcissistic number. A number is narcissistic if the sum of its digits raised to the power of the number of digits equals the number itself.

**Example:**  
```plaintext
Input: 153
Output: True
```

---
## Problem 38: Validate a [Sudoku](https://en.wikipedia.org/wiki/Sudoku) Puzzle

Write a function to validate if a given 9x9 Sudoku board is valid.

**Example:**
```plaintext
Input: [
 [5, 3, ".", ".", 7, ".", ".", ".", "."],
 [6, ".", ".", 1, 9, 5, ".", ".", "."],
 ...
]
Output: True
```

---
## Problem 39: Reverse Digits of a Number

Write a function to reverse the digits of an integer.

**Examples:**  
```plaintext
Input: 12345
Output: 54321

Input: -123
Output: -321
```

---
## Problem 40: Count Lattice Points in a Circle

Write a function to count all integer lattice points `(x, y)` inside or on the boundary of a circle of radius `r`.

**Example:**
```plaintext
Input:  r = 2
Output: 13
```

---
## Problem 41: Implement [Run-Length Encoding](https://en.wikipedia.org/wiki/Run-length_encoding)

Write a function to compress a string using run-length encoding.

**Example:**
```plaintext
Input: "aaabbc"
Output: "a3b2c1"
```

---
## Problem 42: Find Majority Element

Given an array of length `n`, find the majority element. The majority element is the element that appears more than `⌊n/2⌋` times.  
Assume the array always has a majority element.

**Examples:**  
```plaintext
Input:  [3, 2, 3]
Output: 3

Input:  [4, 8, 10, 8, 8, 8, 4]
Output: 8
```

---
## Problem 43: Password Validator

Write a function that validates if a password meets all the following rules:

- Minimum length of 8 characters
- Contains at least one uppercase letter
- Contains at least one lowercase letter
- Contains at least one digit
- Contains at least one special character from @#$%^&*!
- No white-space allowed

**Examples:**
```plaintext
Input: "Pass123!"
Output: True

Input: "weakpass"
Output: False

Input: "NoSpecial123"
Output: False

Input: "Short1!"
Output: False

Input: "Pass 123!"
Output: False (contains space)
```

---
## Problem 44: Find Longest Word in a Sentence

Write a function that takes a sentence as input and returns the longest word. If there are multiple words of the same length, return the first one.

**Examples**
```plaintext
Input: "The quick brown fox jumps over the lazy dog"
Output: "quick"

Input: "I am learning programming"
Output: "programming"
```

---
## Problem 45: Pairs

Implement a function `count_pairs(n, limit)` to determine the number of valid `(x, y)` pairs such that `x + y = n` and integers `x` and `y` satisfy the condition `0 <= x, y <= limit`.  
Assume that `n >= 0`.

**Examples:**

```plaintext
Input: n = 5, limit = 3
Output: 2
Explanation: (2, 3), (3, 2)

Input: n = 7, limit = 5
Output: 4
Explanation: (2, 5), (3, 4), (4, 3), (5, 2)

```

---
## Problem 46: Smallest Even Multiple

Given a positive integer `n`, return the smallest positive integer that is a multiple of both `2` and `n`.

**Examples**

```plaintext
Input: n = 5
Output: 10
Explanation:  
The smallest multiple of both 5 and 2 is 10.

Input: n = 12
Output: 12
Explanation:  
The smallest multiple of both 12 and 2 is 12.
```

---
## Problem 47: Number of Common Factors

Given two positive integers `a` and `b`, return the number of common factors of `a` and `b`.  
An integer `x` is a common factor of `a` and `b` if `x` divides both `a` and `b`.

**Examples:**
```plaintext
Input: a = 12, b = 6
Output: 4
Explanation:  
The common factors of 12 and 6 are 1, 2, 3, 6.

Input: a = 25, b = 30
Output: 2
Explanation:  
The common factors of 25 and 30 are 1, 5.
```

---
## Problem 48: Check [Arithmetic Progression](https://en.wikipedia.org/wiki/Arithmetic_progression)

Given an array of integers, determine if the numbers form an arithmetic progression (a sequence where the difference between consecutive terms is constant).

**Examples**
```plaintext
Input: [3, 7, 11, 15]
Output: True
Explanation: The difference between consecutive terms is 4.

Input: [1, 2, 4]
Output: False
```

---
## Problem 49: Most Frequent Digit

Given a positive integer, determine which digit occurs most frequently. If there is a tie, return the smallest digit.

**Examples**
```plaintext
Input: 112233
Output:  1
Explanation: Digits 1, 2, and 3 occur twice, so the smallest digit (1) is returned.

Input: 9876543211
Output: 1
```

---
## Problem 50: Generate a [Geometric Sequence](https://en.wikipedia.org/wiki/Geometric_progression)

Write a function to generate the first `n` terms of a geometric progression, given the first term `a` and common ratio `r`.

**Examples:**
```plaintext
Input: a = 3, r = 2, n = 5
Output: [3, 6, 12, 24, 48]

Input: a = 1, r = 0.5, n = 4
Output: [1, 0.5, 0.25, 0.125]
```

---
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T416OJAV)