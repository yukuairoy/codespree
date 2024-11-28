---
comments: true
---

# The Birthday Problem
The [birthday problem](https://en.wikipedia.org/wiki/Birthday_problem) asks for the probability that, in a set of $n$ randomly chosen people, at least two will share a birthday[^1]. We assume that birthdays are distributed equally among all days of the year and neglect leap years.

## Mathematical Solution
The probability the first two people have different birthdays is 364/365. The probability that the third person has a birthday different from the first two, given the first two people have different birthdays, is 363/365, and so on. So the probability that all of the first n people have different birthdays is

\[
q(n) = \frac{364}{365}\cdot \frac{363}{365}\cdot \cdots \cdot \frac{365-(n-1)}{365}.
\]

The probability that among $n$ people at least two have the same birthday is $p(n) = 1 - q(n)$.

```python
def get_probability(n: int) -> float:
    q = 1.
    for i in range(1, n):
        q *= (365 - i) / 365
    return 1 - q
```

Let's experiment with various $n$'s:

```python
def experiment():
    for n in (1, 5, 10, 20, 22, 23, 30, 40):
        p = get_probability(n)
        print(f"When n = {n}, p(n) = {p * 100:.1f}%")
```

Output:

```
When n = 1, p(n) = 0.0%
When n = 5, p(n) = 2.7%
When n = 10, p(n) = 11.7%
When n = 20, p(n) = 41.1%
When n = 22, p(n) = 47.6%
When n = 23, p(n) = 50.7%
When n = 30, p(n) = 70.6%
When n = 40, p(n) = 89.1%
```

Observe that the probability of a shared birthday exceeds $50\%$ in a group of only 23 people.

_Question_: In reality, birthdays are not completely random. How might this affect the $p(n)$'s?

## Simulation

The code snippet below is a [Monte Carlo simulation](https://en.wikipedia.org/wiki/Monte_Carlo_method) of the birthday problem.

```python
import random

def has_same_birthday(n: int) -> bool:
    seen = set()
    for _ in range(n):
        birthday = random.randint(1, 365)
        if birthday in seen:
            return True
        seen.add(birthday)
    return False
```

Sample output for $n=23$:

```python
>>> trials = 100_000
>>> n = 23
>>> sum(has_same_birthday(n) for _ in range(trials)) / trials
0.50636
```

## Reverse problem

The reverse problem is to find, for a fixed probability p, the smallest $n$ for which the probability $p(n) \geq p$.

Since $p(n)$ is monotonically increasing, n can be found using **binary search**:

```python
def find_n(p: float) -> int:
    lo, hi = 0, 366
    while lo < hi:
        mid = (lo + hi) // 2
        if get_probability(mid) >= p:
            hi = mid
        else:
            lo = mid + 1
    return lo
```

Testing with $p=0.5$ gives the expected result:

```python
>>> find_n(0.5)
23
```

## Average number of distinct birthdays

The expected number of different birthdays, i.e. the number of days that are at least one person's birthday, can be simulated as follows:

```python
def distinct_birthdays(n: int) -> int:
    birthdays = set()
    for _ in range(n):
        birthday = random.randint(1, 365)
        birthdays.add(birthday)
    return len(birthdays)
```

When there are 1000 people, there will be around 341 different birthdays (around 24 unclaimed birthdays):

```python
>>> trials = 50_000
>>> sum(distinct_birthdays(1000) for _ in range(trials)) / trials)
341.47882
```

The probability that a day is unclaimed by all $n$ days is $(364/365)^n$. The expected number of unclaimed days is thus $365 \cdot \left(\frac{364}{365}\right)^n.$

The expected number of different birthdays is therefore $365 \cdot \left(1 - \left(\frac{364}{365}\right)^n\right).$

When $n=1000$, this number is around $341.5$, which is close to our simulation.

## Number of people until every birthday is achieved

The expected number of people needed until every birthday is achieved is called the [Coupon collector's problem](https://en.wikipedia.org/wiki/Coupon_collector%27s_problem).

Here's a Monte Carlo simulation:

```python
def population_till_all() -> int:
    count = 0
    birthdays = set()
    while len(birthdays) < 365:
        count += 1
        birthday = random.randint(1, 365)
        birthdays.add(birthday)
    return count
```

Sample output:

```python
>>> trials = 50_000
>>> sum(population_till_all() for _ in range(trials)) / trials
2363.53902
```

So on average it takes more than 2360 people to achieve every birthday.

## Average number of people to get at least one shared birthday
What's the average number of people required to find a pair with the same birthday? Below's a simulation:

```python
def till_first_match():
    count = 0
    birthdays = set()
    while True:
        count += 1
        birthday = random.randint(1, 365)
        if birthday in birthdays:
            return count
        birthdays.add(birthday)
```

Sample output:

```python
>>> trials = 50_000
>>> sum(till_first_match() for _ in range(trials)) / trials
24.58436
```

So on average, only 25 people are required to have two people with the same birthday.

[^1]: There is a distinction between birth**day** and birth**date**: the former, except for February 29, occurs each year (e.g. January 15), while the latter is the complete date when a person was born (e.g. January 15, 2001).

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T416OJAV)
