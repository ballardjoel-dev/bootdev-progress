# Functions in Python

Functions encapsulate reusable logic.

Defined with def, followed by the function name and parameters.

Use return to send back a result.

    def area_of_circle(r):
        pi = 3.14
        return pi * r * r

    print(area_of_circle(5))   # 78.5
    print(area_of_circle(10))  # 314.0

Functions help organize code and avoid repetition.

## Functions with Multiple Parameters

Functions can take multiple inputs, separated by commas.

The order of arguments matters — they match the parameter list one by one.

    def create_introduction(name, age, height, weight):
        return f"Your name is {name} and you are {age} years old. You are {height} meters tall and weigh {weight} kilograms."

    intro = create_introduction("Master Chief", "39", "2.2", "450")
    print(intro)
    # Your name is Master Chief and you are 39 years old. You are 2.2 meters tall and weigh 450 kilograms.

Helps when you need to process multiple pieces of data together.

## Function Declaration & Order of Execution

Python runs code top to bottom.

You must declare a function before calling it, unless the call happens after the declaration during runtime.

    def greet(name):
        return f"Hello, {name}!"

    def main():
        print(greet("Alice"))

    main()  # Works — greet is declared before it's called
    
This works too, because greet() is called at runtime, after both functions are defined:

    def main():
        print(greet("Alice"))

    def greet(name):
        return f"Hello, {name}!"

    main()  # Also works

But this will fail:

    def main():
        print(greet("Alice"))

    main()  # NameError: greet is not defined

    def greet(name):
        return f"Hello, {name}!"
        
Functions must be declared before they're called during execution.

## None Return in Python Functions

If a function doesn't have a return statement, it returns None by default.

You can explicitly return None using return None or simply return.

    def greet():
        print("Hello, world!")

    result = greet()
    print(result)  # None (implicit return)

    def farewell():
        print("Goodbye, world!")
    return None

    result = farewell()
    print(result)  # None (explicit return)

    def empty_action():
        print("Attempting to respawn...")
        return

    result = empty_action()
    print(result)  # None (explicit return without expression)

Remember: None signals "no meaningful return value."
