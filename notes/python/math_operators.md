# Mathematical Operators
Basic arithmetic: +, -, *, /

Use parentheses () to control order of operations (PEMDAS)

### Example

    a = 10
    b = 5

    print(a + b)  # 15
    print(a - b)  # 5
    print(a * b)  # 50
    print(a / b)  # 2.0

    # Average with parentheses
    avg = (5 + 7 + 9) / 3
    print(avg)  # 7.0

## Floor Division in Python

Floor division (//) returns the largest whole number less than or equal to the division result (i.e., it discards the remainder and rounds down).

### Examples:

    print(9 // 2)    # 4
    print(-9 // 2)   # -5

## Exponents in Python

Use ** to raise a number to a power. It’s built-in, no imports needed.

### Examples:

    print(3 ** 2)  # 9

    base = 5
    exp = 3
    print(base ** exp)  # 125

## In-Place Operators in Python

In-place operators are shorthand for performing an operation on a variable and updating its value. Common in-place operators include +=, -=, *=, and /=. They simplify code while achieving the same result as a longer assignment.

### Examples

    # Add to variable
    xp = 10
    xp += 5
    print(xp)  # 15

    # Subtract
    gold = 100
    gold -= 20
    print(gold)  # 80

    # Multiply
    damage = 10
    damage *= 2
    print(damage)  # 20

    # Divide
    health = 50
    health /= 2
    print(health)  # 25.0

## Modulo Operator (%) in Python
The modulo operator % returns the remainder after dividing two numbers. It’s commonly used to check properties like whether a number is odd or even.

### Examples

    # Finding remainder
    remainder = 10 % 4
    print(remainder)  # 2

    # Checking if a number is odd
    def is_odd(number):
        return number % 2 != 0

    print(is_odd(3))  # True
    print(is_odd(4))  # False

## Scientific Notation & Readability in Python

Python supports scientific notation for expressing very large or small floats using e or E. It also allows underscores in numeric literals for better readability, making large numbers easier to scan.

### Examples

    # Scientific notation (3 × 10^8)
    light_speed = 3.0e8
    print(light_speed)  # 300000000.0

    # Underscores for readability
    distance_to_moon = 384_400
    print(distance_to_moon)  # 384400
