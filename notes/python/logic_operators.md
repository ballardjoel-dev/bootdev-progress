# Logical Operators in Python

Logical operators like and and or evaluate boolean expressions:

and returns True only if both operands are True

or returns True if at least one operand is True

Parentheses can be used to control evaluation order in complex expressions.

## Examples

    # Using and operator
    has_sword = True
    has_shield = True
    is_warrior = has_sword and has_shield
    print(is_warrior)  # True

    # Using or operator
    is_elf = False
    is_human = True
    is_player = is_elf or is_human
    print(is_player)  # True

    # Nested logical expressions
    is_day = False
    has_torch = True
    can_see = is_day or (not is_day and has_torch)
    print(can_see)  # True

## Not Operator in Python

The not operator is a logical operator that negates a Boolean value. It returns False when applied to True, and True when applied to False. This operator is useful for reversing the logic of conditions.

## Examples:

    is_restricted = True
    print(not is_restricted)
    # False

    is_visible = False
    print(not is_visible)
    # True

## Comparison Operators in Python

Comparison operators are used to evaluate relationships between two values. They return a Boolean result (True or False) and are commonly used in conditionals and control flow.

Common comparison operators:

- < : less than
- > : greater than
- <= : less than or equal to
- >= : greater than or equal to
- == : equal to
- != : not equal to

## Examples

    print(3 < 4)      # True
    print(7 > 8)      # False
    print(10 == 10)   # True
    print(5 != 2)     # True
    print(6 <= 6)     # True
    print(9 >= 10)    # False
