
# Python Dictionaries

A dictionary is an unordered, changeable, and indexed collection of key-value pairs.

## Creating a Dictionary

A dictionary is created using curly braces `{}` or the `dict()` constructor.

```python
car_dict = {
    "brand": "Ford",
    "model": "Mustang",
    "year": 1964
}
```

## Accessing Items

You can access the items of a dictionary by referring to its key name inside square brackets.

```python
brand = car_dict["brand"]
# brand = "Ford"
```

## Modifying Items

You can change the value of a specific item by referring to its key name.

```python
car_dict["year"] = 2018
# car_dict = { "brand": "Ford", "model": "Mustang", "year": 2018 }
```

## Looping Through a Dictionary

You can loop through a dictionary by using a `for` loop. By default, it loops through the keys.

```python
for key in car_dict:
    print(key)
# brand, model, year
```

## Getting Dictionary Values

You can use the `.values()` method to get a view object containing all the values in the dictionary.

```python
v = car_dict.values()
# v = dict_values(['Ford', 'Mustang', 2018])
```

## Getting Key-Value Pairs

You can use the `.items()` method to get a view object of key-value pairs in the dictionary.

```python
items = car_dict.items()
# items = dict_items([('brand', 'Ford'), ('model', 'Mustang'), ('year', 2018)])
```

## Checking for Keys in a Dictionary

To check if a specified key is present in a dictionary, use the `in` keyword.

```python
is_present = "brand" in car_dict
# is_present = True
```

## Dictionary Length

To find out how many items a dictionary has, use the `len()` function.

```python
length = len(car_dict)
# length = 3
```

## Adding Items to a Dictionary

You can add new items to a dictionary by assigning a value to a new key.

```python
car_dict["color"] = "red"
# car_dict = { "brand": "Ford", "model": "Mustang", "year": 2018, "color": "red" }
```

## Removing Items from a Dictionary

You can remove an item from a dictionary using the `pop()` method.

```python
car_dict.pop("model")
# car_dict = { "brand": "Ford", "year": 2018, "color": "red" }
```

## Emptying a Dictionary

To remove all items from a dictionary, use the `clear()` method.

```python
car_dict.clear()
# car_dict = {}
```

## Using the `dict()` Constructor

You can also use the `dict()` constructor to create a dictionary.

```python
car_dict = dict(brand="Ford", model="Mustang", year=1964)
# car_dict = { "brand": "Ford", "model": "Mustang", "year": 1964 }
```

## Nested Dictionaries

A nested dictionary is a dictionary inside another dictionary. You can create a nested dictionary like this:

```python
car_dict = {
    "car1": {
        "brand": "Ford",
        "model": "Mustang",
        "year": 1964
    },
    "car2": {
        "brand": "Chevy",
        "model": "Camaro",
        "year": 1969
    }
}
```

## Using the `dict()` Constructor for Nested Dictionaries

You can also use the `dict()` constructor to create a nested dictionary.

```python
car_dict = dict(
    car1=dict(brand="Ford", model="Mustang", year=1964),
    car2=dict(brand="Chevy", model="Camaro", year=1969)
)
# car_dict = { "car1": { "brand": "Ford", "model": "Mustang", "year": 1964 }, "car2": { "brand": "Chevy", "model": "Camaro", "year": 1969 } }
```
