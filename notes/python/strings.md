# Strings

A string is a sequence of characters enclosed in double qoutes (""). It is a fundamental data type used for representing textual data and can include letters, numbers, symbols, and whitespace.

# F-strings

- F-strings provide a concise and readable way to include variables within strings
- An (f) before the string denotes an f-string
- Any expression within curly brackets {} is evaluated and interpolated into the string
    ## Example 1: Basic use of an f-string
        name = "Thrall"
        age = 28
        print(f"{name} is {age} years old.")
        # Thrall is 28 years old.
    ## Example 2: Incorporating expressions
        a = 5
        b = 10
        print(f"The sum of {a} and {b} is {a + b}.")
        # The sum of 5 and 10 is 15.

  # String Concantation

  - In Python, strings can be concatenated using the + operator. Concatenation involves joining two or more strings end-to-end to form a new string.
    ## Example: Basic string concantation
        first_name = "Boots "
        last_name = "The Bear"
        full_name = first_name + last_name
        print(full_name)
        # Boots The Bear
