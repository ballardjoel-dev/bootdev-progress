# Dictionaries and Sets in Python

## Python Dictionaries

Dictionaries store data as key-value pairs inside curly braces {}. Keys are unique and can be strings, numbers, or tuples, while values can be any data type.

### Examples

### Creating and accessing a dictionary:

    car = {
      "brand": "Toyota",
      "model": "Prius",
      "year": 2019
    }

    print(car["brand"])  # Toyota
    print(car["model"])  # Prius
    print(car["year"])   # 2019

### Modifying, adding, and deleting entries:

    # Modifying a value
    car["year"] = 2021
    print(car["year"])   # 2021

    # Adding a new key-value pair
    car["color"] = "blue"
    print(car["color"])  # blue

    # Deleting a key-value pair
    del car["brand"]
    print(car)  # {'model': 'Prius', 'year': 2021, 'color': 'blue'}

## Checking Key Existence in Python Dictionaries

Use the in keyword to check if a key exists in a dictionary, which helps avoid KeyError when accessing missing keys.

### Examples

    characters = {
        "wizard": "Gandalf",
        "hobbit": "Frodo"
    }

    print("wizard" in characters)  # True
    print("elf" in characters)     # False

## Iterating over a Dictionary in Python

You can loop directly over dictionary keys using a for loop and access each value via its key.

### Examples

    planet_distances = {
        "Mercury": 57.91,
        "Venus": 108.2,
        "Earth": 149.6
    }

    for planet in planet_distances:
        distance = planet_distances[planet]
        print(f"Planet: {planet}, Distance: {distance} million km")

    # Output:
    # Planet: Mercury, Distance: 57.91 million km
    # Planet: Venus, Distance: 108.2 million km
    # Planet: Earth, Distance: 149.6 million km

## Sets in Python

Sets are unordered collections of unique elements. They do not allow duplicates and support operations like union, intersection, and difference. Use set() to create an empty set (not {}, which creates a dictionary). The add() method inserts elements without error on duplicates. Sets can be iterated over but order is not guaranteed.

### Examples

    # Creating and adding to a set
    heroes = {'Ironman', 'Thor', 'Hulk'}
    heroes.add('Spiderman')
    print(heroes)  # {'Hulk', 'Ironman', 'Spiderman', 'Thor'}

    # Removing an element
    heroes.remove('Ironman')
    print(heroes)  # {'Hulk', 'Thor'}

    # Creating an empty set and adding elements
    villains = set()
    villains.add('Loki')
    print(villains)  # {'Loki'}

    # Iterating over a set
    planets = {'Earth', 'Mars', 'Venus'}
    for planet in planets:
        print(planet)
    # Output order may vary

