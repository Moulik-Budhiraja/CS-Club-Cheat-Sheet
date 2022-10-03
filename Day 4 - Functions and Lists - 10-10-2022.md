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
x = [1, 2, 3, 4, 5]
```

We can access individual values in a list using their index. The first value in a list has an index of 0.

```py
x = [1, 2, 3, 4, 5]
print(x[0]) # Prints 1
print(x[1]) # Prints 2
print(x[2]) # Prints 3
print(x[3]) # Prints 4
print(x[4]) # Prints 5
```

We can also access values in a list from the end using negative indexes. The last value in a list has an index of -1.

```py
x = [1, 2, 3, 4, 5]
print(x[-1]) # Prints 5
print(x[-2]) # Prints 4
...
```

We can also change the value of an item in a list.

```py
x = [1, 2, 3, 4, 5]
x[0] = 10
print(x) # Prints [10, 2, 3, 4, 5]
```

We can also add items to a list using the `append()` function.

```py
x = [1, 2, 3, 4, 5]
x.append(6)
print(x) # Prints [1, 2, 3, 4, 5, 6]
```

We can also remove items from a list using the `remove()` function.

```py
x = [1, 2, 3, 4, 5]
x.remove(3)
print(x) # Prints [1, 2, 4, 5]
```

If we want to remove an item from a list using its index we can use the `pop()` function.

```py
x = [1, 2, 3, 4, 5]
x.pop(2)
print(x) # Prints [1, 2, 4, 5]
```

_Note: The `pop()` function returns the value that was removed from the list._

We can also get the length of a list using the `len()` function.

```py
x = [1, 2, 3, 4, 5]
print(len(x)) # Prints 5
```
