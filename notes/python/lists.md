# Lists in Python

Lists are a built-in data structure for storing ordered collections of items. They are defined with square brackets [] and can contain elements of any type, including other lists. Items are comma-separated and lists are mutable, allowing items to be added, removed, or changed.

## Examples

    # Define a list of weapons
    weapons = ["Shortsword", "Iron Dagger", "Elven Bow"]
    print(weapons)
    # ['Shortsword', 'Iron Dagger', 'Elven Bow']

    # Add an item to the list
    inventory = ["Iron Breastplate", "Healing Potion"]
    inventory.append("Shortsword")
    print(inventory)
    # ['Iron Breastplate', 'Healing Potion', 'Shortsword']

## Indexing into Lists in Python

Lists are ordered collections accessed by zero-based indices. The first element is at index 0, the second at index 1, and so forth. This allows direct access to any list item by its position.

## Examples

    names = ["Gordon", "Alyx", "G-man", "Wallace"]

    first_name = names[0]   # "Gordon"
    second_name = names[1]  # "Alyx"
    last_name = names[3]    # "Wallace"

## List Length in Python

The length of a list is found using the len() function, which returns the number of elements. Note that list indices start at 0, so the length is always one more than the last index.

## Examples

    characters = ["Frodo", "Sam", "Gandalf"]
    total_characters = len(characters)
    print(total_characters)  # 3

## Updating List Elements in Python

Lists are mutable, so you can change their elements by accessing them via index and assigning a new value.

## Examples

    inventory = ["Leather", "Iron Ore", "Healing Potion"]
    inventory[0] = "Leather Armor"
    print(inventory)
    # ['Leather Armor', 'Iron Ore', 'Healing Potion']

## Appending and Popping Items in Python Lists

The append() method adds an item to the end of a list, modifying it in place. The pop() method removes and returns the last item by default, or an item at a specified index if provided.

## Examples

    # Appending items
    fruits = []
    fruits.append("apple")
    fruits.append("banana")
    fruits.append("cherry")
    print(fruits)  # ['apple', 'banana', 'cherry']

    # Popping the last item
    heroes = ["Iron Man", "Captain America", "Thor", "Hulk"]
    last_hero = heroes.pop()
    print(heroes)    # ['Iron Man', 'Captain America', 'Thor']
    print(last_hero) # 'Hulk'

    # Popping an item at a specific index
    removed_hero = heroes.pop(1)
    print(heroes)       # ['Iron Man', 'Thor']
    print(removed_hero) # 'Captain America'

## Iterating Directly Over List Items in Python

You can loop through a list’s elements directly using for item in list syntax, which accesses each element without needing its index. This simplifies code when you only need the values.

## Examples

    fruits = ['apple', 'banana', 'cherry']
    for fruit in fruits:
        print(fruit)
    # apple
    # banana
    # cherry

## Slicing Lists in Python

List slicing extracts a portion of a list using the syntax my_list[start:stop:step].

- start: index to begin (inclusive)
- stop: index to end (exclusive)
- step: interval between elements

All parts are optional and can be negative to count from the end.

## Examples

    # Slice with start, stop, step
    scores = [10, 20, 30, 40, 50, 60, 70]
    print(scores[2:6:2])  # [30, 50]

    # Omitting start or stop
    numbers = list(range(10))
    print(numbers[:3])  # [0, 1, 2]
    print(numbers[3:])  # [3, 4, 5, 6, 7, 8, 9]

    # Using only step
    numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9]
    print(numbers[::3])  # [1, 4, 7]

    # Negative indices
    print(numbers[-4:])  # [6, 7, 8, 9]

## List Concatenation in Python

Lists can be combined using the + operator, which joins elements from multiple lists into one.

## Examples

    heroes = ["Superman", "Batman"]
    villains = ["Joker", "Lex Luthor"]
    characters = heroes + villains
    print(characters)
    # ['Superman', 'Batman', 'Joker', 'Lex Luthor']

## List Operations - Contains

Use the in keyword to check if an item exists in a list. It returns True if the item is present, otherwise False.

## Examples

    heroes = ["Spiderman", "Ironman", "Thor"]
    print("Thor" in heroes)    # True
    print("Batman" in heroes)  # False

## List Deletion in Python

The del keyword removes items from a list by index or slice. It can also clear the entire list.

## Examples

    # Delete element by index
    heroes = ["Thor", "Iron Man", "Captain America", "Hulk"]
    del heroes[1]
    print(heroes)  # ['Thor', 'Captain America', 'Hulk']

    # Delete a slice of elements
    heroes = ["Thor", "Iron Man", "Captain America", "Hulk"]
    del heroes[1:3]
    print(heroes)  # ['Thor', 'Hulk']

    # Delete all elements in the list
    heroes = ["Thor", "Iron Man", "Captain America", "Hulk"]
    del heroes[:]
    print(heroes)  # []

