# List of primes (functions)

Before, you wrote `check-prime.py`, a program that checks whether a single number is a prime. In this assignment you turn that check into a function, and then use that function to build a list of primes.

Create a file called `list_primes.py`. You are not going to ask the user for input: test your functions with hard-coded calls, like in the examples below.

## Part 1: is_prime

Define a function `is_prime(x)` that returns `True` if `x` is a prime number, and `False` otherwise. Start from the loop in your `check-prime.py`.

Remember that 1 is not a prime number.

### Example Usage

    print(is_prime(7))
    print(is_prime(9))
    print(is_prime(2))
    print(is_prime(1))

### Expected Output

    True
    False
    True
    False

## Part 2: list_primes

Define a function `list_primes(n)` that returns a list of all primes $$p$$ with $$2 \leq p < n$$, in ascending order.

Call `is_prime` inside `list_primes` to decide whether a number goes into the list. Do not repeat the prime-checking loop — that is exactly what the function is for.

### Example Usage

    print(list_primes(10))
    print(list_primes(11))
    print(list_primes(30))

### Expected Output

    [2, 3, 5, 7]
    [2, 3, 5, 7]
    [2, 3, 5, 7, 11, 13, 17, 19, 23, 29]

## Constraints

* You are *not* allowed to use the `break`-statement.
* You are *not* allowed to use the `import`-statement.

## Run

Run your program and verify that it indeed displays the expected text:

    python list_primes.py

## Checkpy

You can use checkpy to verify that it meets our requirements:

    checkpy list_primes
