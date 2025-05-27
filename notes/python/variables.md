# Variables and Basic Types in Python

## Variables
Store data using = (assignment operator).

Names reference the stored values.

Can hold any data type.


        my_height = 100
        my_name = "James Holden"

## Basic Types

- String: Text in single ' or double " quotes.
- Integer: Whole numbers (positive or negative).
- Float: Numbers with decimals.
- Boolean: True or False.

        name = "boot.dev"    # String
        x = 5                # Integer
        y = -3.2             # Float
        is_active = True     # Boolean
  
## F-strings (String Interpolation)

Use f"" syntax to embed variables or expressions directly in strings.

    age = 28
    print(f"{name} is {age} years old.")  # boot.dev is 28 years old

    a = 5
    b = 10
    print(f"The sum of {a} and {b} is {a + b}")  # The sum of 5 and 10 is 15

## NoneType and None in Python

None represents no value or null.

Different from 0, False, or "" (empty string).

Often used as a default or placeholder value.

    empty_var = None  # NoneType

    none_val = None         # NoneType
    none_string = "None"    # String, not NoneType
