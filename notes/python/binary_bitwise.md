# Binary and Bitwise

## Binary Numbers

Binary numbers represent values using base 2, consisting only of digits 0 and 1. This is fundamental in computing, as all data in computers is processed in binary. Each digit corresponds to a power of 2, similar to how decimal digits represent powers of 10.

## Examples:

- 0001 in binary equals 1 in decimal.
- 0110 in binary equals 6 in decimal.
- 1111 in binary equals 15 in decimal.

## Bitwise “&” Operator in Python

The bitwise "&" operator performs an "and" operation on each pair of corresponding bits from two numbers. For each bit pair, the result is 1 if both bits are 1; otherwise, it is 0.

In Python, binary numbers are prefixed with 0b, distinguishing them from decimal numbers. Bitwise operations are commonly used for managing binary flags or permissions efficiently.

## Examples

    # Permissions
    can_create_guild = 0b1000
    can_review_guild = 0b0100
    can_delete_guild = 0b0010
    can_edit_guild = 0b0001

    # User permissions: can_review_guild and can_edit_guild
    user_permissions = 0b0101

    # Checking for can_review_guild permission
    has_review_permission = user_permissions & can_review_guild
    print(has_review_permission == can_review_guild)  # True

    # Checking for can_create_guild permission
    has_create_permission = user_permissions & can_create_guild
    print(has_create_permission == can_create_guild)  # False

## Bitwise OR Operator in Python

The bitwise OR operator | performs a logical OR operation on each pair of corresponding bits of two binary numbers. Each bit in the result is set to 1 if at least one of the corresponding bits in the operands is 1; otherwise, it is set to 0. This is useful for combining flags or permissions represented in binary.

## Examples

    a = 0b0101  # 5 in binary
    b = 0b0111  # 7 in binary

    result = a | b
    print(bin(result))  # 0b111

    # Combining guild permissions using bitwise OR
    can_invite = 0b1000  # Permission to invite
    can_kick = 0b0100    # Permission to kick

    guild_permissions = can_invite | can_kick
    print(bin(guild_permissions))  # 0b1100
