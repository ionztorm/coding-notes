# Day 1: Beginner - Working with Variables to Manage Data

## Contents

- [Printing](#printing)
  - [Basics](#basics)
  - [Printing on multiple lines](#printing-on-multiple-lines)
  - [Adding (concatenating) strings](#adding-concatenating-strings)
- [Input](#input)
- [Variables](#variables)
  - [Basics](#basics)
  - [Naming conventions](#naming-conventions)
  - [Geting the length of a string](#geting-the-length-of-a-string)
- [Day 1 Project: Band Name Generator](#day-1-project-band-name-generator)
  - [Instructions](#instructions)

---

## Printing

### Basics

- **print** is a function that prints the value of a variable to the console.
- It can take multiple arguments and prints them in the order they are passed.
- For text stings, you can use single or double quotes.

```python
print("Hello, World!")
# Output: Hello, World!
```

### Printing on multiple lines

- You can use the **\n** character to print on multiple lines.

```python
print("Hello\nWorld!")
# Output: Hello
#         World!
```

### Adding (concatenating) strings

- You can concatenate strings using the **+** operator.

```python
print("Hello" + " " + "World!")
# Output: Hello World!
```
## Input

### Basics

- **input** is a function that takes user input and returns it as a string.
- You can pass a prompt message to the function.

```python
input("Enter your name: ")
# Output: Enter your name:
```

## Variables

### Basics

- A variable is a container that stores data.
- You can assign a value to a variable using the **=** operator.

```python
name = input("Enter your name: ")
print("Hello, " + name + "!")
# Output: Enter your name: John
#         Hello, John!
```

### Naming conventions

- Variable names can contain letters, numbers, and underscores.
- They cannot start with a number.
- They are case-sensitive.
- They use snake_case naming convention.

```python
first_name = "Johngit@github.com:cli/cli.git"
last_name = "Doe"
age = 25
is_student = True
```

### Geting the length of a string

- You can use the **len** function to get the length of a string.

```python
name = input("Enter your name: ")
print("Your name has " + len(name) + " characters.")
# Output: Enter your name: John
#         Your name has 4 characters.
```
