# Tuples in Python

Tuples store ordered, immutable collections of elements defined with parentheses (). They can hold mixed data types and support indexing. Unlike lists, tuples cannot be changed after creation. Tuple unpacking allows assigning elements to variables in one statement. You can concatenate tuples to create new ones.

### Examples

### Creating and accessing tuple elements:

wizard = ("Gandalf", 2019, True)
print(wizard[0])  # Gandalf
print(wizard[1])  # 2019
print(wizard[2])  # True

### Tuple unpacking:

hero = ("Aragorn", 87)
hero_name, hero_age = hero
print(hero_name)  # Aragorn
print(hero_age)   # 87

### List of tuples and accessing nested elements:

characters = [("Frodo", 50, True), ("Sam", 38, True)]
print(characters[0][0])  # Frodo
print(characters[1][1])  # 38

### Appending to a tuple via concatenation:

original_tuple = (1, 2, 3)
addition = (4,)
new_tuple = original_tuple + addition
print(new_tuple)  # (1, 2, 3, 4)
