# Functions and Lists

#### 10-10-2022

---

[Back to Table of Contents](/README.md)

### Functions

Functions are used to store code that can be reused. We have already used a few functions, such as `print()` and `input()`. We can also create our own functions. Functions are defined using the `def` keyword.

```py
def my_function():
    print("Hello World")
```

We can then call the function using its name.

```py
my_function() # Prints "Hello World"
```

Functions can also take arguments. Arguments are values that are passed into the function.

```py
def my_function(name):
    print("Hello " + name)
```

We can then call the function using its name and passing in an argument.

```py
my_function("Bob") # Prints "Hello Bob"
```

Functions can also return values. For example the `input()` function returns the value that the user enters. We can use the `return` keyword to return a value from a function.

```py
def add(x, y):
    return x + y
```

We can then call the function and store the result in a variable.

```py
result = add(5, 5)
print(result) # Prints 10
```

### Lists

Lists are used to store multiple values. Lists are surrounded by square brackets and each value is separated by a comma.

```py
lst1 = [1, 2, 3, 4, 5]

# Lists can contain multiple data types
lst2 = ["Bob", "Alice", "John"]

# Lists can mix and match data types
lst3 = [1, "Bob", True]

# Lists can contain other lists
lst4 = [[1, 2, 3], [4, 5, 6]]

# Lists can be empty
lst5 = []
```

_Note: we use cannot make the name of a variable `list` as it is already a built-in function. This is why we use "lst" as a generic name for our lists_

#### Accessing and Changing List Values

We can access individual values in a list using their index. The first value in a list has an index of 0.

```py
lst = [1, 2, 3, 4, 5]
print(lst[0]) # Prints 1
print(lst[1]) # Prints 2
print(lst[2]) # Prints 3
print(lst[3]) # Prints 4
print(lst[4]) # Prints 5
```

We can also access values in a list from the end using negative indexes. The last value in a list has an index of -1.

```py
lst = [1, 2, 3, 4, 5]
print(lst[-1]) # Prints 5
print(lst[-2]) # Prints 4
...
```

We can also change the value of an item in a list.

```py
lst = [1, 2, 3, 4, 5]
lst[0] = 10
print(lst) # Prints [10, 2, 3, 4, 5]
```

#### List Methods

Lists have a number of useful methods that can be used to manipulate them.

_Recall: A **method** is called upon on an existing object and generally manipulates that object. ie. `object.method()`_

`append()` - Adds an item to the end of the list.

```py
lst = [1, 2, 3, 4, 5]
lst.append(6)
print(lst) # Prints [1, 2, 3, 4, 5, 6]
```

`remove()` - Removes an item from the list.

```py
lst = [1, 2, 3, 4, 5]
lst.remove(3)
print(lst) # Prints [1, 2, 4, 5]
```

`pop()` - Removes an item from the list and returns it.

```py
lst = [1, 2, 3, 4, 5]
y = lst.pop(2)
print(lst) # Prints [1, 2, 4, 5]
print(y) # Prints 3
```

### Length

We can get the length of a list using the `len()` function.

```py
lst = [1, 2, 3, 4, 5]
print(len(lst)) # Prints 5
```

The `len()` function can also be used on strings.

```py
s = "Hello World"
print(len(s)) # Prints 11
```
