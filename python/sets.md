
# Python Sets

A set is a collection in Python that is unordered, unindexed, and does not allow duplicate elements.

## Creating a Set

A set is created using curly braces `{}` or the `set()` constructor. 

Curly braces cannot be used to create an empty set since they are also used to create dictionaries.

```python
my_set = {1, 2, 3, 4}
# my_set = {1, 2, 3, 4}
```

Alternatively, you can use the `set()` constructor to create a set.

```python
my_set = set([1, 2, 3, 4])
# my_set = {1, 2, 3, 4}
```

## Accessing Items in a Set

Sets are unordered, meaning you cannot access elements by index or key. You can loop through the set using a `for` loop.

```python
for item in my_set:
    print(item)
# Output: 1, 2, 3, 4 (order is not guaranteed)
```

## Adding Items to a Set

You can add a single element to a set using the `.add()` method.

```python
my_set.add(5)
# my_set = {1, 2, 3, 4, 5}
```

To add multiple elements, use the `.update()` method.

```python
my_set.update([6, 7, 8])
# my_set = {1, 2, 3, 4, 5, 6, 7, 8}
```

## Removing Items from a Set

You can remove an item from a set using the `.remove()` method. This method will raise an error if the item is not found.

```python
my_set.remove(4)
# my_set = {1, 2, 3, 5, 6, 7, 8}
```

To remove an item without causing an error if it doesn't exist, use the `.discard()` method.

```python
my_set.discard(4)
# my_set = {1, 2, 3, 5, 6, 7, 8}  (no error if 4 is not found)
```

You can also use the `.pop()` method to remove and return a random item.

```python
item = my_set.pop()
# Randomly removes and returns an item
```

## Clearing a Set

To remove all items from a set, use the `.clear()` method.

```python
my_set.clear()
# my_set = set()  (empty set)
```

## Set Length

To determine how many items a set has, use the `len()` function.

```python
length = len(my_set)
# length = 4
```

## Set Operations

Sets support various operations, including union, intersection, difference, and symmetric difference.

### Union

The union of two sets can be obtained using the `.union()` method or the `|` operator.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
union_set = set1.union(set2)
# union_set = {1, 2, 3, 4, 5}
# Or using the | operator
union_set = set1 | set2
# union_set = {1, 2, 3, 4, 5}
```

### Intersection

The intersection of two sets can be obtained using the `.intersection()` method or the `&` operator.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
intersection_set = set1.intersection(set2)
# intersection_set = {3}
# Or using the & operator
intersection_set = set1 & set2
# intersection_set = {3}
```

### Difference

The difference between two sets can be obtained using the `.difference()` method or the `-` operator.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
difference_set = set1.difference(set2)
# difference_set = {1, 2}
# Or using the - operator
difference_set = set1 - set2
# difference_set = {1, 2}
```

### Symmetric Difference

The symmetric difference between two sets can be obtained using the `.symmetric_difference()` method or the `^` operator.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
sym_diff_set = set1.symmetric_difference(set2)
# sym_diff_set = {1, 2, 4, 5}
# Or using the ^ operator
sym_diff_set = set1 ^ set2
# sym_diff_set = {1, 2, 4, 5}
```

## Set Membership

To check if an item exists in a set, use the `in` keyword.

```python
is_present = 3 in my_set
# is_present = True
```

## Copying a Set

To create a copy of a set, use the `.copy()` method.

```python
set_copy = my_set.copy()
# set_copy = {1, 2, 3, 4}
```

## Frozen Set

A frozen set is an immutable version of a set. It can be created using the `frozenset()` constructor.

```python
frozen_set = frozenset([1, 2, 3, 4])
# frozen_set = frozenset({1, 2, 3, 4})
```

A frozen set does not support methods like `.add()`, `.remove()`, etc., since it is immutable.


