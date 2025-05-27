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
