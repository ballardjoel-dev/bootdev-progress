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

