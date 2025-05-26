# Find Factorial

## Assignment

Complete the factorial() function. It should return the factorial of a given number.

- A factorial is the product (multiplication result) of all positive integers less than or equal to a given number.

## Example
- 1! = 1 = 1
- 2! = 2 * 1 = 2
- 3! = 3 * 2 * 1 = 6
- 4! = 4 * 3 * 2 * 1 = 24
- 5! = 5 * 4 * 3 * 2 * 1 = 120

There is also a special case for zero:

- 0! = 1

## Start
    def factorial(num):
        pass
## Solution

    def factorial(num):
        result = 1
        for i in range(1, num + 1):
            result *= i
        return result
