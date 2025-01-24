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
* Practicing unit testing, a crucial skill for software engineering.

---

## Problem 1: Vowel Counter

Write a program that counts the number of vowels in a given word. Vowels are `a`, `e`, `i`, `o`, `u` (case-insensitive).

**Examples:**
```
Input: "hello"
Output: 2

Input: "EducaTiOn"
Output: 5

Input: "rhytHm"
Output: 0

Input: "aQuAriUm"
Output: 5

Input: "PYTHON"
Output: 1

Input: "cOmpUtEr"
Output: 3

Input: "12345abc"
Output: 1

Input: ""
Output: 0

Input: "aeiouAEIOU"
Output: 10

Input: "sTrAwbErrY"
Output: 2
```

---

## Problem 2: Reverse a List

Write a function to reverse a list of numbers.

**Examples:**  
```
Input: [1, 2, 3, 4, 5]
Output: [5, 4, 3, 2, 1]

Input: [10, 20, 30]
Output: [30, 20, 10]

Input: []
Output: []

Input: [7]
Output: [7]

Input: [1, 1, 1, 1]
Output: [1, 1, 1, 1]

Input: [-1, -2, -3, -4]
Output: [-4, -3, -2, -1]

Input: [0, 100, 200]
Output: [200, 100, 0]

Input: [3, 5, 2, 9]
Output: [9, 2, 5, 3]

Input: [42]
Output: [42]

Input: [8, 6, 7, 5, 3, 0, 9]
Output: [9, 0, 3, 5, 7, 6, 8]
```

---

## Problem 3: String Reversal

Write a function to reverse a string.

**Examples:**  
```
Input: "hello"
Output: "olleh"

Input: ""
Output: ""

Input: "madam"
Output: "madam"

Input: "hello world!"
Output: "!dlrow olleh"

Input: "  abc  "
Output: "  cba  "

Input: "Python"
Output: "nohtyP"
```

---

## Problem 4: Perfect Square

Check if a number is a [perfect square](https://en.wikipedia.org/wiki/Square_number). A perfect square is a non-negative integer that is the square of another integer.

**Examples:**
```
Input: 25
Output: True
Explanation: 25 (5 * 5 = 25)

Input: 18
Output: False

Input: 0
Output: True (0 * 0 = 0)

Input: 4
Output: True

Input: 15
Output: False

Input: 16
Output: True

Input: 101
Output: False

Input: 10000
Output: True

Input: -1
Output: False (A perfect square must be non-negative)
```

---

## Problem 5: Second Largest

Find the second largest number in an array.  
Assume that the input array contains at least two numbers.

**Examples:**
```
Input: [10, 5, 8, 12]
Output: 10

Input: [1, 2, 3, 4, 5]
Output: 4

Input: [5, 5, 5, 5]
Output: 5

Input: [5, 3, 0, 5]
Output: 5

Input: [1, 2]
Output: 1

Input: [-1, -2, -3]
Output: -2

Input: [5, 10, 15, 20, 25]
Output: 20

Input: [3, 1, 4, 2]
Output: 3

Input: [0, -1, -2, -3]
Output: -1

Input: [42, 35, 35, 42, 35, 35]
Output: 42
```

---

## Problem 6: [Digital Root](https://en.wikipedia.org/wiki/Digital_root)

Add all digits in a number until you get a single digit.

**Examples:**
```
Input: 789
Output: 6 (7+8+9=24, 2+4=6)

Input: 1234
Output: 1 (1+2+3+4=10, 1+0=1)

Input: 5
Output: 5

Input: 100
Output: 1
Explanation: 1 + 0 + 0 = 1.

Input: 456
Output: 6
Explanation: 4 + 5 + 6 = 15, 1 + 5 = 6.

Input: 1001
Output: 2
Explanation: 1 + 0 + 0 + 1 = 2.

Input: 98765
Output: 8
Explanation: 9 + 8 + 7 + 6 + 5 = 35, 3 + 5 = 8.

Input: 123456789
Output: 9
Explanation: 1 + 2 + 3 + 4 + 5 + 6 + 7 + 8 + 9 = 45, 4 + 5 = 9.

Input: 999999999
Output: 9
Explanation: 9 repeated 9 times adds up to 81, 8 + 1 = 9.
```

---

## Problem 7: Extra Character

Given two strings, `A` and `B`, where `A` is a string that contains all the characters of `B` in the same order, plus exactly one additional character at a random position, find the extra character in `A`.

**Examples:**  
```
Input: A = "atcb42c", B = "atb42c"
Output: "c"

Input: A = "abcd", B = "abc"
Output: "d"

Input: A = "aabbcc", B = "aabcc"
Output: "b"

Input: A = "xylophone", B = "xylophne"
Output: "o"

Input: A = "12345", B = "1234"
Output: "5"

Input: A = "a", B = ""
Output: "a"

Input: A = "HellO", B = "HelO"
Output: "l"
```

---

## Problem 8: Number Triangle

Print a triangle pattern of numbers where each row contains increasing numbers starting from 1.

**Examples:**
```
Input: 1
Output:
1

Input: 3
Output:
1
1 2
1 2 3

Input: 5
Output:
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5

Input: 7
Output:
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
1 2 3 4 5 6
1 2 3 4 5 6 7
```

---

## Problem 9: Longest Common Prefix

Write a function to find the longest prefix shared by all strings in an array. A **prefix** is the beginning part of a string. For example, the prefixes of "car" are "c", "ca", and "car".

If no common prefix exists, return an empty string "".

**Examples:**:
```
Input: ["beaux", "beauty", "beat", "beam"]
Output: "bea"

Input: ["apple", "ape", "april"]
Output: "ap"

Input: ["test", "testing", "tester"]
Output: "test"

Input: ["hello", "world", "python"]
Output: ""

Input: ["short", "longer", "different"]
Output: ""

Input: ["prefix", "preference", ""]
Output: ""

Input: ["test", "test", "test"]
Output: "test"

Input: []
Output: ""

Input: ["fun"]
Output: "fun"
```

---

## Problem 10: Split Array with Two Sets

Given an integer array, the task is to determine whether it can be split into two parts such that each part contains only distinct elements.

**Examples:**  
```
Input: [10, 10, 20, 20, 30, 40]
Output: True
Explanation: One possible split into [10, 20, 30] and [10, 20, 40].
Both parts have distinct elements.

Input: [1, 1, 1, 1]
Output: False

Input: [1, 2, 3, 4, 5, 6]
Output: True
Explanation: One possible split is [1, 2, 3] and [4, 5, 6].

Input: [1, 1, 1, 2, 2, 2]
Output: False
Explanation: No way to split into two parts with distinct elements in each.

Input: [1]
Output: True
Explanation: The array can be split into [1] and an empty set.

Input: []
Output: True
Explanation: An empty array trivially satisfies the condition.

Input: [6, 6]
Output: True
Explanation: The array can be split as [6] and [6].

Input: [3, 4, 3, 4]
Output: True
Explanation: The array can be split as [3, 4] and [3, 4].
```

---

## Problem 11: Reverse Words

Given a sentence, reverse the order of words. Trim leading and trailing spaces, and reduce multiple spaces to a single space between words.

**Examples:**
```
Input: "The quick brown fox"
Output: "fox brown quick The"

Input: "Hello world!"
Output: "world! Hello"

Input: "  Python   is   fun  "
Output: "fun is Python"

Input: "Single"
Output: "Single"
```

---

## Problem 12: Find the Missing Number

Given an array containing `n` distinct numbers taken from the range `[0, n]`, find the missing number.

**Examples:**
```
Input: [3, 0, 1]
Output: 2

Input: [2, 3, 1, 4, 5]
Output: 0
```

---

## Problem 13: Rearrange Vowels

Write a function to rearrange the vowels in a string in alphabetical order, placing uppercase vowels before lowercase vowels. Keep all consonants in their original positions.

**Examples:**
```
Input: s = "coding"
Output: "cidong"

Input: s = "AaEeIiOoUu"
Output: "AEIOUaeiou"

Input: s = "alphabet"
Output: "alphabet"

Input: s = "alphabEt"
Output: "Elphabat"
```

---

## Problem 14: First Unique Character

Given a string, find the index of the first unique character. Return `-1` if no such character exists.

**Examples:**  
```
Input: "lastlasp"
Output: 3

Input: "sophhpho"
Output: 0
```

---

## Problem 15: Reverse Digits of a Number

Write a function to reverse the digits of an integer.

**Examples:**  
```
Input: 12345
Output: 54321

Input: -123
Output: -321
```

---

## Problem 16: Minimum Common Value

You are given two sorted integer arrays, `nums1` and `nums2`. Both are in non-decreasing order. Find the smallest integer that appears in both arrays. If there is no common element, return `-1`.

**Examples:**
```
Input: nums1 = [1, 2, 3], nums2 = [2, 4]
Output: 2

Input: nums1 = [1, 2, 3, 6], nums2 = [2, 3, 4, 4]
Output: 2

Input: nums1 = [1, 3, 5], nums2 = [2, 4, 6]
Output: -1
```

---

## Problem 17: Add Two Numbers Represented as Strings

Write a function to add two numbers represented as strings. Return the sum as a string.

**Examples:**  
```
Input: num1 = "123", num2 = "456"
Output: "579"

Input: num1 = "999", num2 = "1"
Output: "1000"
```

---

## Problem 18: Sum of Array Except Self

Given an array of integers, return a new array such that each element at index `i` is the sum of all numbers in the original array except the one at `i`.

**Examples:**  
```
Input: [1, 2, 3, 4, 5]
Output: [14, 13, 12, 11, 10]

Input: [3, 2, 1]
Output: [3, 4, 5]
```

---

## Problem 19: Largest Sum of Non-Adjacent Numbers

Given a list of integers, write a function that returns the largest sum of two non-adjacent numbers.

**Examples:**  
```
Input: [2, 4, 6, 8]
Output: 12 (4+8)

Input: [5, 1, 1, 5]
Output: 10 (5+5)
```

---

## Problem 20: [Power Function](https://en.wikipedia.org/wiki/Exponentiation)

Implement the function `pow(x, y)` to compute $x^y$.

**Examples:**
```
Input: x = 2, y = 3
Output: 8

Input: x = 5, y = -2
Output: 0.04
```

---

## Problem 21: [Combinations](https://en.wikipedia.org/wiki/Combination)

Write a function to compute the number of ways to choose `k` items from `n` items (combinations), denoted as $C(n, k)$.

**Examples:**
```
Input: n = 5, k = 2
Output: 10

Input: n = 6, k = 3
Output: 20
```

---

## Problem 22: Check for [Palindrome](https://en.wikipedia.org/wiki/Palindrome)

Write a function to check if a given string is a palindrome.

**Examples:**
```
Input:  "madam"
Output: True

Input: "hello"
Output: False
```

---

## Problem 23: Check if Two Strings are [Anagrams](https://en.wikipedia.org/wiki/Anagram)

Write a function to check if two strings are anagrams of each other.

**Examples:**  
```
Input: "listen", "silent"
Output: True

Input: "apple", "pale"
Output: False
```

---

## Problem 24: Check If a Number is [Prime](https://en.wikipedia.org/wiki/Prime_number)

Write a function to determine if a given number is prime.

**Examples:**  
```
Input: 13
Output: True

Input: 10
Output: False
```

---

## Problem 25: Phone Number Formatter

Write a program that formats a 10-digit phone number into the format `(XXX) XXX-XXXX`.

**Examples:**
```
Input: "1234567890"
Output: "(123) 456-7890"

Input: "9876543210"
Output: "(987) 654-3210"
```

---

## Problem 26: Array Rotation

Rotate an array by `k` positions to the right.

**Examples:**
```
Input: [1, 2, 3, 4], k = 2
Output: [3, 4, 1, 2]

Input: [10, 20, 30, 40, 50], k = 3
Output: [30, 40, 50, 10, 20]

Input: [1, 2, 3], k = 0
Output: [1, 2, 3]

Input: [1, 2, 3], k = 3
Output: [1, 2, 3]

Input: [10, 20, 30, 40, 50], k = 1
Output: [50, 10, 20, 30, 40]

Input: [], k = 3
Output: []

Input: [7, 8, 9], k = 10
Output: [9, 7, 8]
```

---

## Problem 27: FizzBuzz String

Write a function `fizzbuzz_string(n)` that returns a single string containing the FizzBuzz sequence from 1 to `n`, separated by commas.

* For multiples of 3, use "Fizz".
* For multiples of 5, use "Buzz".
* For multiples of both 3 and 5, use "FizzBuzz".
* Otherwise, just use the number itself.

**Example:**  
```
Input: 15
Output: "1,2,Fizz,4,Buzz,Fizz,7,8,Fizz,Buzz,11,Fizz,13,14,FizzBuzz"
```

---

## Problem 28: Diamond Pattern

Print a diamond pattern using asterisks (`*`).

**Examples:**
```
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

A **pangram** is a sentence that contains every letter of the English alphabet at least once.  
Write a function to determine whether a given string is a pangram. The check should be case-insensitive.

**Examples:**
```
Input: "The quick brown fox jumps over the lazy dog"
Output: True

Input: "Pack my box with five dozen liquor jugs 1234!!!"
Output: True
Explanation: Numbers and punctuation are ignored, and all letters are present at least once.

Input: "The quick brown fox jumps over the la dog"
Output: False
```

---

## Problem 30: Largest Alphabetical Rotation

Given a string `s`, generate all rotations (cyclic shifts) of `s` and return the **lexicographically largest** rotation.

**Examples:**
```
Input: "abc"
Rotations: "abc", "bca", "cab"
Output: "cab"

Input: "zab"
Rotations: "zab", "abz", "bza"
Output: "zab"  # since "zab" is lexicographically largest among "zab", "abz", "bza"
```

---

## Problem 31: Date String Formatter

Write a function `reformat_date(date_str)` that takes a string in the format `YYYY-MM-DD` and returns a string in the format `MonthName DD, YYYY`, where `MonthName` is the full English month (e.g., "January", "February", …).

**Examples:**
```
Input: "2023-01-15"
Output: "January 15, 2023"

Input: "1999-12-31"
Output: "December 31, 1999"
```

---

## Problem 32: Compute [Double Factorial](https://en.wikipedia.org/wiki/Double_factorial)

Write a function that computes the double factorial of a given non-negative integer `n`.  
The double factorial of `n`, denoted as `n!!`, is defined as the product of all integers from 1 to `n` that have the same parity (odd or even) as `n`.  

**Examples:**
```
Input: n = 8
Output: 384
Explanation: 8!! = 8 * 6 * 4 * 2 = 384

Input: n = 7
Output: 105
Explanation: 7!! = 7 * 5 * 3 * 1 = 105
```

---

## Problem 33: Partition String into Fixed-Size Groups

Given a string `s`, an integer `k`, and a fill character `fill`, partition `s` into groups of size `k`. If the length of `s` is not a multiple of `k`, pad the final group with the fill character until it has size `k`. Return all the groups as a list of strings.

**Examples:**
```
Input: s = "hello", k = 2, fill = "*" 
Output: ["he", "ll", "o*"]
Explanation: The remainder has only 'o', so we add one '*' to form a group of size 2.

Input: s = "abcd123", k = 3, fill = "-"
Output: ["abc", "d12", "3--"]
Explanation: String length is 7, so we need 2 fill characters '-' to complete the last group.
```

---

## Problem 34: Check [Perfect Number](https://en.wikipedia.org/wiki/Perfect_number)

Write a function to check if a number is a perfect number. A perfect number is a positive integer equal to the sum of its proper divisors (excluding itself).

**Example:**
```
Input: 6
Output: True
```

---

## Problem 35: Pattern Matching

You have a string `s` and a pattern `p` containing exactly one `'*'`. The `'*'` can match any sequence of zero or more characters. Determine whether it is possible to replace the `'*'` in `p` with some (possibly empty) string such that the resulting string becomes a substring of `s`. Return true if such a match exists, otherwise false.

**Examples:**
```
Input: s = "abanana", p = "b*na"
Output: true
Explanation: '*' can match "ana", giving "banana" which is a substring of "abanana".

Input: s = "aaaa", p = "b*a"
Output: false
Explanation: There is no substring in "aaaa" that starts with 'b'. Hence, no match.

Input: s = "luck", p = "u*"
Output: true
Explanation: Possible replacements for '*' ("", "c", "ck") lead to substrings "u", "uc",
or "uck" in "luck".
```

---

## Problem 36: Check [Derangement](https://en.wikipedia.org/wiki/Derangement)

Write a function to check if one permutation of a string is a derangement of another. A derangement means no character appears in its original position.

**Examples:**
```
Input: s1 = "abc", s2 = "cab"
Output: True

Input: s1 = "abc", s2 = "bac"
Output: False
```

---

## Problem 37: Check [Narcissistic Number](https://en.wikipedia.org/wiki/Narcissistic_number)

Write a function to check if a number is a narcissistic number. A number is narcissistic if the sum of its digits raised to the power of the number of digits equals the number itself.

**Example:**
```
Input: 153
Output: True (1^3+5^3+3^3=153)
```

---

## Problem 38: Validate a [Sudoku](https://en.wikipedia.org/wiki/Sudoku) Puzzle

Write a function to validate if a given 9x9 Sudoku board is valid.

**Examples:**
```
Input:
[
 ["5", "3", ".", ".", "7", ".", ".", ".", "."],
 ["6", ".", ".", "1", "9", "5", ".", ".", "."],
 [".", "9", "8", ".", ".", ".", ".", "6", "."],
 ["8", ".", ".", ".", "6", ".", ".", ".", "3"],
 ["4", ".", ".", "8", ".", "3", ".", ".", "1"],
 ["7", ".", ".", ".", "2", ".", ".", ".", "6"],
 [".", "6", ".", ".", ".", ".", "2", "8", "."],
 [".", ".", ".", "4", "1", "9", ".", ".", "5"],
 [".", ".", ".", ".", "8", ".", ".", "7", "9"]
]
Output: True

Input:
[
 ["5", "3", ".", ".", "7", ".", ".", ".", "."],
 ["6", ".", ".", "1", "9", "5", ".", ".", "."],
 [".", "9", "8", ".", ".", ".", ".", "6", "."],
 ["8", ".", ".", ".", "6", ".", ".", ".", "3"],
 ["4", ".", ".", "8", ".", "3", ".", ".", "1"],
 ["7", ".", ".", ".", "2", ".", ".", ".", "6"],
 [".", "6", ".", ".", ".", ".", "2", "8", "."],
 [".", ".", ".", "4", "1", "9", ".", ".", "5"],
 [".", ".", "9", ".", "8", ".", ".", "7", "9"] 
]
Output: False
Explanation: The last row has two '9's (positions [8][2] and [8][8]).

Input:
[
 [".", ".", "4", ".", ".", ".", ".", ".", "."],
 [".", ".", ".", ".", ".", ".", "5", ".", "."],
 [".", ".", ".", ".", "7", ".", ".", "2", "."],
 [".", ".", ".", "8", ".", ".", ".", ".", "9"],
 [".", ".", ".", ".", ".", "1", ".", ".", "."],
 [".", ".", ".", ".", ".", ".", ".", ".", "."],
 [".", "9", ".", ".", ".", ".", ".", "1", "."],
 [".", ".", ".", ".", ".", ".", ".", ".", "."],
 [".", ".", ".", "8", ".", ".", ".", ".", "."]
]
Output: False
Explanation: There's an '8' in row 3 (0-indexed) and row 8 (0-indexed), both in the same column.

Input:
[
 [".", ".", ".", ".", ".", "5", ".", ".", "."],
 [".", ".", "3", "1", ".", ".", ".", ".", "."],
 [".", ".", "8", ".", ".", ".", ".", "6", "."],
 ["5", ".", ".", ".", "6", ".", ".", ".", "3"],
 ["4", ".", ".", "8", ".", "3", ".", ".", "1"],
 ["7", ".", ".", ".", "2", ".", ".", ".", "6"],
 [".", "6", ".", ".", ".", ".", "2", "8", "."],
 [".", ".", ".", "4", "1", "9", ".", ".", "5"],
 [".", ".", ".", ".", "8", ".", ".", "7", "3"]
]
Output: False
```

---

## Problem 39: Count Unique Characters in a String

Write a function that counts the number of unique characters in a string.

**Examples:**
```
Input: "programming"
Output: 8

Input: "hello"
Output: 4
```

---

## Problem 40: Lattice Points in a Circle

Write a function to count all integer lattice points `(x, y)` inside or on the boundary of a circle of radius `r`.

**Example:**
```
Input: r = 2
Output: 13
Explanation: They are
  (-2, 0), (-1, -1), (-1, 0), (-1, 1), (0, -2), (0, -1),
  (0, 0), (0, 1), (0, 2), (1, -1), (1, 0), (1, 1), (2, 0)
```

---

## Problem 41: [Run-Length Encoding](https://en.wikipedia.org/wiki/Run-length_encoding)

Write a function to compress a string using run-length encoding.

**Example:**
```
Input: "aaabbc"
Output: "a3b2c1"

Input: "xxxytttttttzxxqqqqqqqqqq"
Output: "x3y1t7z1x2q10"
```

---

## Problem 42: Majority Element

Given an array of length `n`, find the majority element. The majority element is the element that appears more than `⌊n/2⌋` times.  
Assume the array always has a majority element.

**Examples:**
```
Input: [3, 2, 3]
Output: 3

Input: [4, 8, 10, 8, 8, 8, 4]
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
```
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

## Problem 44: Prime Factors of a Number

Write a function to count the number of prime factors of a given positive integer. A prime factor is a prime number that divides the given number exactly.

**Examples:**
```
Input: 60
Output: 3
Explanation: The prime factors of 60 are 2, 3, and 5.

Input: 100
Output: 2
Explanation: The prime factors of 100 are 2 and 5.

Input: 37
Output: 1
Explanation: The prime factor of 37 is 37 itself.

Input: 1
Output: 0
Explanation: 1 has no prime factors.

Input: 84
Output: 3
Explanation: The prime factors of 84 are 2, 3, and 7.
```

---

## Problem 45: Pairs

Implement a function `count_pairs(n, limit)` to determine the number of valid `(x, y)` pairs such that `x + y = n` and integers `x` and `y` satisfy the condition `0 <= x, y <= limit`.  
Assume that `n >= 0`.

**Examples:**
```
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

**Examples:**
```
Input: n = 5
Output: 10
Explanation: The smallest multiple of both 5 and 2 is 10.

Input: n = 12
Output: 12
Explanation: The smallest multiple of both 12 and 2 is 12.
```

---

## Problem 47: Common Factors

Given two positive integers `a` and `b`, return the number of common factors of `a` and `b`.  
An integer `x` is a common factor of `a` and `b` if `x` divides both `a` and `b`.

**Examples:**
```
Input: a = 12, b = 6
Output: 4
Explanation: The common factors of 12 and 6 are 1, 2, 3, 6.

Input: a = 25, b = 30
Output: 2
Explanation: The common factors of 25 and 30 are 1, 5.
```

---

## Problem 48: [Arithmetic Progression](https://en.wikipedia.org/wiki/Arithmetic_progression)

Given an array of integers, determine if the numbers form an arithmetic progression (a sequence where the difference between consecutive terms is constant).

**Examples:**
```
Input: [3, 7, 11, 15]
Output: True
Explanation: The difference between consecutive terms is 4.

Input: [1, 2, 4]
Output: False
```

---

## Problem 49: Most Frequent Digit

Given a positive integer, determine which digit occurs most frequently. If there is a tie, return the smallest digit.

**Examples:**
```
Input: 112233
Output:  1
Explanation: Digits 1, 2, and 3 occur twice, so the smallest digit (1) is returned.

Input: 9876543211
Output: 1
```

---

## Problem 50: [Geometric Sequence](https://en.wikipedia.org/wiki/Geometric_progression)

Write a function to generate the first `n` terms of a geometric progression, given the first term `a` and common ratio `r`.

**Examples:**
```
Input: a = 3, r = 2, n = 5
Output: [3, 6, 12, 24, 48]

Input: a = 1, r = 0.5, n = 4
Output: [1, 0.5, 0.25, 0.125]
```

---

## Problem 51: Truncated Mean

Write a function to calculate the truncated mean of a list of integers. The truncated mean is the average of the numbers in the list after removing the smallest and largest values. If there are multiple occurrences of the smallest or largest value, only one instance of each is removed.  
Assume that the size of the input array is at least three.

**Examples:**
```
Input: [2, 3, 4, 5, 6]
Output: 4
Explanation: Removing the smallest (2) and largest (6) values leaves [3, 4, 5].
The mean is (3 + 4 + 5) / 3 = 4.

Input: [1, 2, 3, 2, 3, 1]
Output: 2
Explanation: Removing one smallest (1) and one largest (3) value leaves [1, 2, 2, 3].
The mean is (1 + 2 + 2 + 3) / 4 = 2.
```

---

## Problem 52: Sort by Age

Given two arrays - one containing `names` and another containing corresponding `ages` - write a function to sort people by their ages in _descending_ order. Return the sorted list of names.  
Assume the values of `ages` are distinct.

**Examples:**
```
Input: names = ["Alice", "Bob", "Charlie"], ages = [24, 45, 70]
Output: ["Charlie", "Bob", "Alice"]

Input: names = ["Mark", "Emma", "Alex", "Sarah"], ages = [75, 18, 41, 65]
Output: ["Mark", "Sarah", "Alex", "Emma"]
```

---

## Problem 53: Partition Number

Given a positive integer `n`, find the partition integer `x` where the sum of all integers from 1 to `x` equals the sum of all integers from `x` to `n`.  
If no such integer exists, return `-1`.

**Examples:**
```
Input: 8
Output: 6
Explanation: 1 + 2 + 3 + 4 + 5 + 6 = 6 + 7 + 8

Input: 49
Output: 35
Explanation: 1 + 2 + ... + 35 = 35 + 36 + ... + 49

Input: 1
Output: 1
Explanation: 1 is the pivot integer since 1 = 1

Input: 15
Output: -1
Explanation: No such integer exist
```

---

## Problem 54: Smallest String After One Swap

You are given a string `str`. In one operation, you can swap any two characters at adjacent positions.
Your task is to return the [alphabetically](https://en.wikipedia.org/wiki/Alphabetical_order) smallest string that can be obtained by performing exactly one swap operation on the string.

**Examples:**
```
Input: "deed"
Output: "dede"

Input: "abcd"
Output: "abcd"
Explanation: Any swap would result in a alphabetically larger string

Input: "alphabet"
Output: "alhpabet"
```

---

## Problem 55: Word Chain

A list of words is valid if each word starts with the last letter of the previous word. Write a function to check if the given sequence of words is valid.  
Assume the words are case-insensitive.

**Examples:**
```
Input: ["hello", "orange", "elephant", "tree"]
Output: True
Explanation: "hello" -> "orange" -> "elephant" -> "tree".

Input: ["cat", "dog", "pig", "goat"]
Output: False
Explanation: "dog" does not start with "t".

Input: ["Apple", "Elephant", "tiger"]
Output: True
Explanation: Case is ignored, so "Apple" -> "Elephant" -> "tiger" is valid.

Input: ["zebra"]
Output: True
Explanation: A single word is trivially valid.

Input: []
Output: True
Explanation: An empty list is trivially valid.
```

---

## Problem 56: Detect Cyclic Words

Write a function to check if two strings are cyclic permutations of each other. Two strings are cyclic permutations if one string can be rotated to match the other.

**Examples:**
```
Input: s1 = "abcde", s2 = "deabc"
Output: True
Explanation: Rotating "deabc" gives "abcde".

Input: s1 = "hello", s2 = "lohel"
Output: True

Input: s1 = "hello", s2 = "lolhe"
Output: False
```

---

## Problem 57: Find Missing Page Number

Imagine you are given a book where pages are labeled from 1 to `n` , but one page is missing. Write a function to find the missing page number from a given list of page numbers.  
Assume the input is _sorted_.

**Examples:**
```
Input: [1, 2, 3, 4, 6]
Output: 5

Input: [2, 3, 4, 5]
Output: 1
```

**Bonus:** Can we solve this problem faster than [linear time](https://en.wikipedia.org/wiki/Time_complexity#Linear_time)?

---

## Problem 58: Alternating Sum of Digits

Write a function to calculate the alternating sum of digits in an integer. Alternate between adding and subtracting each digit from left to right.

**Examples:**
```
Input: 12345
Output: 1 - 2 + 3 - 4 + 5 = 3

Input: 9876
Output: 9 - 8 + 7 - 6 = 2
```

---

## Problem 59: Palindromic Chain

A sequence of words is a **palindromic chain** if the words form a palindrome when read as a continuous sentence (ignoring spaces and punctuation). Write a function to check if a list of words forms a palindromic chain.

**Examples:**
```
Input: ["madam", "im", "adam"]
Output: True
Explanation: Combining the words gives "madamimadam", which is a palindrome.

Input: ["hello", "world"]
Output: False
Explanation: "helloworld" is not a palindrome.

Input: ["race", "car"]
Output: True
Explanation: "racecar" is a palindrome.
```

---

## Problem 60: Longest Increasing Subarray

A **subarray** is a _contiguous_ portion of an array. For example, in the array `[1, 2, 3, 4]`, `[1, 2]` and `[3, 4]` are subarrays, but `[1, 3]` is not because the elements are not contiguous.

Write a function to find the length of the longest subarray in a list of integers where the elements are strictly increasing.

**Examples:**
```
Input: [1, 2, 3, 1, 2]
Output: 3
Explanation: The subarray [1, 2, 3] is the longest increasing subarray.

Input: [5, 1, 2, 3, 0]
Output: 3
Explanation: The subarray [1, 2, 3] is the longest.
```

---

## Problem 61: Peak Indices

You are given a 0-indexed integer array, `nums`. You need to find all indices `i` (except the first and last) such that `nums[i] > nums[i - 1]` and `nums[i] > nums[i + 1]`.

**Examples:**
```
Input: [1, 4, 3, 8, 5]
Output: [1, 3]
Explanation: nums[0] and nums[4] cannot be peaks because they are
the first and last elements. nums[1] and nums[3] are strictly greater
than their neighboring elements.

Input: [2, 4, 4]
Output: []
Explanation: nums[0] and nums[2] cannot be peaks because they are
the first and last elements. nums[1] also can not be a peak because
it is not strictly greater than nums[2].

Input: [5, 2, 3, 1, 4]
Output: [2]

Input: [1, 2, 3, 2, 1]
Output: [2]
```

---

## Problem 62: Longest Monotonic Subarray

You are given a 0-indexed integer array, `nums`. A subarray is a contiguous portion of the array. We say a subarray is:

* Strictly Increasing if each element is greater than the one before it.
* Strictly Decreasing if each element is less than the one before it.

Your task is to find the length of the longest subarray that is strictly increasing or strictly decreasing.

**Examples:**
```
Input: [2, 2, 2]
Output: 1
Explanation: No two consecutive elements are strictly increasing or strictly decreasing,
so the longest valid subarray is just any single element.

Input: [1, 2, 3, 4]
Output: 4
Explanation: The entire array [1, 2, 3, 4] is strictly increasing.

Input: [5, 6, 5, 4, 3, 10]
Output: 4
Explanation: [6, 5, 4, 3] is strictly decreasing (length 4).

Input: [1, 3, 5, 4, 2]
Output: 3
```

---

## Problem 63: K-th Fibonacci Number

Find the `k`-th [Fibonacci number](https://en.wikipedia.org/wiki/Fibonacci_sequence).

**Examples:**
```
Input: k = 1
Output: 1

Input: k = 2
Output: 1

Input: k = 3
Output: 2

Input: k = 4
Output: 3

Input: k = 5
Output: 5

Input: k = 10
Output: 55
```

---

## Problem 64: Largest Positive Integer With Its Negative

You are given an integer array `nums` (which contains no zero). Your task is to find the largest positive integer `k` such that both `k` and `-k` exist in `nums`. If no such integer exists, return `-1`.

**Examples:**
```
Input: [-1, 10, 6, 7, -7, 1]
Output: 7

Input: [-10, 8, 6, 7, -2, -3, 8]
Output: -1

Input: [-3, -2, 2, 3]
Output: 3
```

---

## Problem 65: Desk Phone Transfer

There are `n` desks in a row, labeled from 0 to `n-1`. At time `0`, desk `0` receives an important phone call. Each second, the call is transferred to the next desk in ascending order. Once it reaches the last desk (`n-1`), it reverses direction and moves back toward desk `0`. This back-and-forth pattern continues indefinitely. Given a time `k` (in seconds), determine which desk the call is at exactly at time `k`.

**Examples:**
```
Input: n = 4, k = 5
Output: 1
Explanation: Desks are labeled 0, 1, 2, 3. At each second:
  Time 0: Desk 0
  Time 1: Desk 1
  Time 2: Desk 2
  Time 3: Desk 3
  Time 4: Desk 2
  Time 5: Desk 1
After 5 seconds, the call is at desk 1.

Input: n = 3, k = 7
Output: 1
Explanation: Desks are labeled 0, 1, 2. At each second:
  Time 0: Desk 0
  Time 1: Desk 1
  Time 2: Desk 2
  Time 3: Desk 1
  Time 4: Desk 0
  Time 5: Desk 1
  Time 6: Desk 2
  Time 7: Desk 1
After 7 seconds, the call is at desk 1.
```

---

## Problem 66: Perfect Square

Given an `n x n` grid where each cell contains an integer from `1` to `n`, determine whether **every row** and **every column** contains **all** integers from `1` to `n`.

**Examples:**
```
Input: [[1, 2, 3], [3, 1, 2], [2, 3, 1]]
Output: True
Explanation: In this case, n = 3, and every row and column contains the
numbers 1, 2, and 3.

Input: [[1, 2, 2], [3, 1, 2], [2, 3, 1]]
Output: False
Explanation: In this case, n = 3, but the first row has a repeated 2.
```