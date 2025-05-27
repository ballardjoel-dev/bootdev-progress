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
  
## Strings, Concatenation & F-strings

Strings are sequences of characters, written in single ' or double " quotes.

You can concatenate strings using the + operator:

    first_name = "Boots "
    last_name = "The Bear"
    full_name = first_name + last_name
    print(full_name)  # Boots The Bear
 
 ## Prefer f-strings for readability, especially when combining text and variables:

    name = "Boots"
    age = 4
    print(f"{name} is {age} years old.")  # Boots is 4 years old

F-strings are more concise, easier to read, and support expressions directly inside {}.

## Multiple Variable Assignment

You can assign multiple variables in one line by separating them with commas:

    sword_name, sword_damage, sword_length = "Excalibur", 10, 200

This is useful for setting related values together.

## NoneType and None in Python

None represents no value or null.

Different from 0, False, or "" (empty string).

Often used as a default or placeholder value.

    empty_var = None  # NoneType

    none_val = None         # NoneType
    none_string = "None"    # String, not NoneType

## Dynamic Typing in Python

Python variables can change type at runtime; no need to declare types upfront.

Different from statically typed languages, which require fixed types and catch errors earlier.

    value = 10       # integer
    value = "ten"    # now a string

    # Recommended: use new variables for clarity
    value = 10
    value_description = "ten"
