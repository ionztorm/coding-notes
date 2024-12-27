
# Python Loops

## The For Loop

```python
for item in list_of_items:
    do something to each item
```

- For example:

```python
fruits = ["apple", "banana", "pear"]

for fruit in fruits:
    print(fruit)
# apple
# banana
# pear
```

### For .. in range ..

- We can also use the `for... in range ..` loop:

```python
for item in range(a,b):
    do something to each item
```

- The `range` keyword accepts 3 arguments:

  1. The start - optional with a default of 0. Specifies at which position to start.
  2. The end - required. Specifies at which point to end.
  3. The step - optional with a default of 1. Specifies the increment at which item increases.

- Note that the `end` is not inclusive. Similar to accessing list indexes, the end specifies which number to stop before.

```python
for i in range(6):
    print(i)
# prints numbers 0 - 5

for i in range(3,20):
    print(i)
# prints numbers 3 - 19

for i in range(2,20,2):
    print(i)
# prints 2, 4, 6, 8, 10, 12, 14, 16, 18
```

