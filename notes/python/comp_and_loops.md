# Comparisons and Loops

## If-Else Statements in Python

if-elif-else statements let your program choose between multiple code paths based on different conditions. Python evaluates each condition in order:

The first True condition runs its block.

If none are True, the else block runs (if included).

### Example:

    def check_age_group(age):
        if age >= 65:
            return "Senior"
        elif age >= 18:
            return "Adult"
        elif age >= 13:
            return "Teenager"
        else:
            return "Child"

    print(check_age_group(70))  # Senior
    print(check_age_group(15))  # Teenager

## For Loops in Python

for loops in Python are used to iterate over sequences or ranges of values, making it easy to perform repetitive tasks like processing each item in a list or counting through numbers.

### For Loops with range()

The range() function generates a sequence of numbers, which is commonly used in for loops. It can take up to three arguments: a start value, a stop value, and an optional step value. The sequence starts at the start value (inclusive), stops before the stop value (exclusive), and increments by the step value.

### Iterating from 0 to 4

    for i in range(5):
        print(i)
    # Output:
    # 0
    # 1
    # 2
    # 3
    # 4

### Iterating from 2 to 6 with custom logic

    for i in range(2, 7):
        doubled = i + i
        print(doubled)
    # Output:
    # 4
    # 6
    # 8
    # 10
    # 12

### Using a positive step value

    for i in range(1, 10, 2):
        print(i)
    # Output:
    # 1
    # 3
    # 5
    # 7
    # 9
    
### Using a negative step value to iterate backwards

    for i in range(5, 0, -1):
        print(i)
    # Output:
    # 5
    # 4
    # 3
    # 2
    # 1

## While Loops in Python

A while loop repeats a block of code as long as a condition is True. It’s useful when the number of iterations isn't known in advance.

Make sure the condition will eventually become False to avoid infinite loops.

### Example:

    counter = 1
    while counter <= 3:
        print(f"Counter: {counter}")
        counter += 1

    # Output:
    # Counter: 1
    # Counter: 2
    # Counter: 3
