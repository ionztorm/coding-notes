# Lists

<!--toc:start-->

- [Lists](#lists)
  - [Basics](#basics)
    - [Define a List](#define-a-list)
    - [Adding and Removing Items](#adding-and-removing-items)
    - [Looping Through a List](#looping-through-a-list)
  - [List Slicing](#list-slicing)
  <!--toc:end-->

## Basics

### Define a List

- Lists are defined using [].

```py
list_name = [item1, item2, item3]
```

### Adding and Removing Items

- Add items to the list using `.append()`

```py
list_name.append(item4)
```

- Remove the last item from the list using `.pop()`

```py
list_name.pop()
```

- We can store the value removed by `.pop()` in a variable.

```py
removed_item = list_name.pop()
```

- Remove an item from the list using `.remove()`

```py
list_name.remove(item3)
```

- We can also remove an item by its index using `del`

```py
del list_name[1]
```

- We can also remove an item by its index using `pop`

```py
list_name.pop(1)
```

### Looping Through a List

- Loop through the list using a for loop.

```py
for  item in list_name:
    print(item)
```

## List Slicing

- We can slice a list using the following syntax:

```py
list_name[start:stop:step]
```

- `start` is the index of the first item we want to include in the slice.
- `stop` is the index of the first item we don't want to include in the slice.
- `step` is the number of items to skip.
- If we don't specify `start`, `stop`, or `step`, the default values are `0`, `len(list_name)`, and `1` respectively.
- We can also use negative indices to slice the list from the end.
- We can also use `[::-1]` to reverse the list.

```py
list_name[-1] # last item in the list
```

```py
list_name[::-1] # reverse the list, for example, [1, 2, 3] will become [3, 2, 1]
```

```py
list_name[::2] # get every second item in the list
```

```py
list_name[1:4] # get items from index 1 to but not including index 4
```

```py
list_name[1:] # get items from index 1 to the end of the list
```

```py
list_name[:3] # get items from the start of the list to but not including index 3
```
