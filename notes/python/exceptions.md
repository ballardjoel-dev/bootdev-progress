# Errors and Exceptions in Python

Errors in Python fall into two categories:

- Syntax Errors: Mistakes in code structure that prevent parsing (e.g., missing colons or invalid keywords). Detected before the code runs.
- Exceptions: Runtime errors that occur during execution. These can be handled with try-except blocks to prevent program crashes.

Use try to wrap risky code, except to define how to handle specific or general exceptions, and as to capture exception details.

You can raise exceptions manually using raise to signal issues like invalid input. Avoid handling the exception in the same function—let the calling code handle it with try-except.

Always catch specific exceptions before general ones (Exception) to handle known error types cleanly. Catch-all except blocks should come last.

## Examples

    # Syntax error (won't run)
    # this is not valid code

    # Handling a general exception
    try:
        result = 10 / 0
    except Exception as e:
        print(f"Error encountered: {e}")
    # Output: Error encountered: division by zero

    # Raising and handling custom exceptions
    def forge_weapon(material):
        if material not in ["bronze", "iron", "steel"]:
            raise Exception("invalid material for weapon crafting")
        return f"{material} weapon"

    try:
        forge_weapon("wood")
    except Exception as e:
        print(e)
    # Output: invalid material for weapon crafting

    # Raising when item not found
    def find_item(item_id, items):
        if item_id not in items:
            raise Exception("item id not found")
        return items[item_id]

    inventory = {'sword': 1, 'shield': 2}
    try:  
        find_item('bow', inventory)
    except Exception as e:
        print(e)
    # Output: item id not found

    # Handling specific exceptions
    try:
        result = 10 / 0
    except ZeroDivisionError:
        print("Cannot divide by zero.")
    except Exception as e:
        print(f"Unexpected error: {e}")

    try:
        animals = ["dragon", "unicorn"]
        print(animals[3])
    except IndexError:
        print("Index error occurred: List index out of range.")
    except Exception as e:
        print(f"Unexpected error: {e}")
        
