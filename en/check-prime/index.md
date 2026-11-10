# Check prime

A prime number is an integer number $$n$$ that can not be divide by any other integer number (other than $$1$$ and $$n$$ itself). Implement a program called `check-prime.py`, that checks if a given number is a prime number.

    Enter a number: 7
    7 is a prime number!

    Enter a number: 9
    9 is not a prime number.

## Background

As previously mentioned, a computer is a great tool for quickly executing a series of "dumb", or simple, actions. An example of what a computer does a lot better (and quicker!) than humans, is calculating prime numbers. The definition of a prime number is not too complicated. But determining how many divisors a number has could take an enormous amount of time. Python to the rescue!

## Constraints

You cannot use all tools available in Python, just yet. There are some constraints:

* You are only allowed to use the concepts that are discussed in this module.
* You are *not* allowed to use the `break`-statement.
* You are *not* allowed to use the `import`-statement.

## Problem analysis

This problem is a bit more complicated than the problems you've had before. It's good to take a couple of minutes of time, before any coding, to work out the problem with **pen and paper**. Try to answer these questions:

- How would you divide the problem into smaller and simpler steps?
- Can you think of intermediate steps that are easier? (For instance, print for each number smaller than $$n$$ if it is a divisor or not.)

### Hint

At the start, keep it simple. Use a `for`-loop and `%` (modulo) to determine how many numbers are a divisor of `number`. If you keep track of this in the loop (count!), then by the end of the loop you can determine if a number is prime or not. Ultimately print the conclusion, like in the example above.

## Run

If you're doing it right you're continuously testing your code by running it:

    python check-prime.py

## Testing

To be sure test your program again using `checkpy`:

    checkpy check-prime
