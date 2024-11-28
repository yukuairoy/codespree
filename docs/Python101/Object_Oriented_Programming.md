---
comments: true
---

# Object-Oriented Programming

## Introduction

Object-Oriented Programming (OOP) is a paradigm that emphasizes organizing software design around data, or objects, instead of functions and logic. This approach allows for more natural modeling of real-world scenarios within the programming context.

### Defining Classes and Objects

A class serves as a blueprint for objects, encapsulating attributes (data) and methods (functions) that operate on that data. Consider the `Cat` class as an example:

```python
class Cat:
    species = "Felis catus"  # Class attribute

    def __init__(self, name, age):
        self.name = name  # Instance attribute
        self.age = age

    def description(self):
        return f"{self.name} is {self.age} years old"

    def speak(self, sound):
        return f"{self.name} says {sound}"
```

Instantiation and interaction with a Cat object:

```python
my_cat = Cat("Cookie", 8)
print(my_cat.description())  # Output: Cookie is 8 years old
print(my_cat.speak("meow"))  # Output: Cookie says meow
```

### Inheritance: Enhancing Reusability and Hierarchy

Inheritance is a fundamental principle of object-oriented programming that enables a class to derive or inherit attributes and behaviors (methods) from another class. This mechanism promotes code reusability and establishes a natural hierarchy among classes.

In the following example, the `Persian` class inherits from the `Cat` class. This means that a `Persian` cat is a specialized form of `Cat` that retains general `Cat` behaviors while also defining behaviors specific to Persian cats.

```python
class Persian(Cat):
    def speak(self, sound="purr"):
        return super().speak(sound)
```

In this code:

- The `Persian` class extends `Cat`, meaning it inherits `Cat`'s attributes and methods.
- The `speak` method in the `Persian` class overrides the same method in the `Cat` class, providing a specific behavior for Persian cats. The `super()` function is used to call the parent class's method, allowing the `Persian` class to extend or modify its behavior.

### Encapsulation: Data Integrity

Encapsulation promotes data integrity by restricting direct access to an object's attributes. It's not just about making attributes private; it's about providing controlled access through public methods.

```python
class Cat:
    def __init__(self, name, age):
        self.__name = name  # Private attribute
        self.__age = age    # Private attribute

    # Getter and setter methods for name
    def get_name(self):
        return self.__name

    def set_name(self, name):
        self.__name = name

    # Getter and setter methods for age
    def get_age(self):
        return self.__age

    def set_age(self, age):
        if age < 0:
            raise ValueError("Age cannot be negative.")
        else:
            self.__age = age
```

Usage:

```python
my_cat = Cat("Whiskers", 5)
my_cat.set_name("Mr. Whiskers")
my_cat.set_age(-1)  # Raises Error
my_cat.set_age(6)
print(my_cat.description())  # Output: Mr. Whiskers is 6 years old
```

### Polymorphism: Interface Flexibility

Polymorphism allows objects of different classes to be treated through a common interface.

```python
class Siamese(Cat):
    def speak(self, sound="meezer"):
        return super().speak(sound)

def cat_speak(cat: Cat):
    print(cat.speak())

siamese = Siamese("Luna", 3)
persian = Persian("Ginger", 5)

cat_speak(siamese)  # Output: Luna says meezer
cat_speak(persian)  # Output: Ginger says purr
```

## Examples

### Design a Social Media Platform

Design a simplified model for a social media platform that captures interactions between users, posts, and comments.

**Solution**:

```python
class User:
    def __init__(self, username):
        self.username = username
        self.posts = []

    def create_post(self, content):
        post = Post(self, content)
        self.posts.append(post)
        return post

class Post:
    def __init__(self, user, content):
        self.user = user
        self.content = content
        self.comments = []

    def add_comment(self, content, user):
        comment = Comment(user, content)
        self.comments.append(comment)
        return comment

class Comment:
    def __init__(self, user, content):
        self.user = user
        self.content = content

# Usage
user1 = User("john_doe")
post = user1.create_post("Hello, world!")
user2 = User("jane_smith")
comment = post.add_comment("Nice post!", user2)

print(f"{comment.user.username} commented on {post.user.username}'s post: {comment.content}")
```

### Design an ATM System

Create a simplified ATM system allowing users to perform transactions like balance inquiries and cash withdrawals.

**Solution**:

```python
class User:
    def __init__(self, card_number, pin, account):
        self.card_number = card_number
        self.pin = pin
        self.account = account

class Account:
    def __init__(self, balance):
        self.balance = balance

    def withdraw(self, amount):
        if amount > self.balance:
            print("Insufficient balance.")
            return False
        self.balance -= amount
        print(f"Withdrew ${amount}. New balance: ${self.balance}.")
        return True

    def check_balance(self):
        print(f"Account balance: ${self.balance}")

class ATM:
    def __init__(self, users):
        self.users = users  # Dictionary: card number -> User object

    def authenticate_user(self, card_number, pin):
        user = self.users.get(card_number)
        if user and user.pin == pin:
            return user
        return None

    def handle_transaction(self, user, transaction_type, amount=None):
        if transaction_type == 'balance_inquiry':
            user.account.check_balance()
        elif transaction_type == 'withdrawal':
            user.account.withdraw(amount)
        else:
            print("Invalid transaction type.")

# Usage example
account = Account(1000)
user = User("12345678", "1234", account)
atm = ATM({"12345678": user})

authenticated_user = atm.authenticate_user("12345678", "1234")
if authenticated_user:
    atm.handle_transaction(authenticated_user, 'balance_inquiry')
    atm.handle_transaction(authenticated_user, 'withdrawal', 500)
```

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T416OJAV)