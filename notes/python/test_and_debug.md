# Testing and Debugging

## Unit Testing in Python

Unit tests verify small pieces of code (usually functions) in isolation.

They compare a function’s actual return value with the expected result.

Unit testing helps catch bugs early and ensures code behaves as intended.

## Stack Traces in Python

A stack trace (or traceback) shows the sequence of function calls leading to an error.

It includes:

- File name
- Line number
- Function or code block
- Error type and message

It helps locate and understand what caused a program to fail.

    def greet(name):
        print(f"Hello, {name}")
      print("Welcome!")  # Indentation mismatch

    greet("Arwen")
    
### Example Error:

    File "example.py", line 4
        print("Welcome!")
        ^
    IndentationError: unindent does not match any outer indentation level
