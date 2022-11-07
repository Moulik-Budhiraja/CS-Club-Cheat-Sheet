# Functions and Strings

#### 17-10-2022

---

[Back to Table of Contents](/README.md)

## In this lesson

-   [Functions](#functions)
    -   [Defining a Function](#defining-a-function)
    -   [Parameters](#parameters)
    -   [Return Values](#return-values)
-   [Strings](#strings)
    -   [Indexing and Slicing](#indexing-and-slicing)
    -   [String Methods](#string-methods)
    -   [Useful Methods](#useful-methods)

### Functions

#### Defining a Function

Functions are used to store code that can be reused. We have already used a few functions, such as `print()` and `input()`. We can also create our own functions. Functions are defined using the `def` keyword.

```py
def my_function():
    print("Hello World")
```

We can then call the function using its name.

```py
my_function() # Prints "Hello World"
```

#### Parameters

Functions can also take arguments. Arguments are values that are passed into the function.

```py
def my_function(name):
    print("Hello " + name)
```

We can then call the function using its name and passing in an argument.

```py
my_function("Bob") # Prints "Hello Bob"
```

#### Return Values

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

### Strings

As we have seen before, strings are a sequence of characters. Strings can be created using single quotes, double quotes or triple-double quotes (for multi-line strings).

```py
my_string = "Hello World"
my_string = 'Hello World'
my_string = """Hello World"""
```

#### Indexing and Slicing

We can access individual characters in a string using indexing. Indexing starts at 0 and goes up to the length of the string minus 1.

```py
my_string = "abcd"
print(my_string[0]) # Prints "a"
print(my_string[1]) # Prints "b"
print(my_string[2]) # Prints "c"
print(my_string[3]) # Prints "d"
```

We can also access characters from the end of the string using negative indexing.

```py
my_string = "abcd"
print(my_string[-1]) # Prints "d"
print(my_string[-2]) # Prints "c"
print(my_string[-3]) # Prints "b"
print(my_string[-4]) # Prints "a"
```

_Notice that negitive indexing begins at `-1` and not `0`_

We can also access a range of characters in a string using slicing. Slicing uses the syntax `string[start:end:step]`. The start index is included and the end index is not included.

```py
my_string = "abcd"
print(my_string[0:2]) # Prints "ab"
print(my_string[1:3]) # Prints "bc"
print(my_string[2:4]) # Prints "cd"
```

We can also omit the start and end indexes. If we omit the start index, it defaults to the start of the string. If we omit the end index, it defaults to the end of the string.

```py
my_string = "abcd"
print(my_string[:2]) # Prints "ab"
print(my_string[1:]) # Prints "bcd"
print(my_string[:]) # Prints "abcd"
```

We can also use negative indexes in slicing.

```py
my_string = "abcd"
print(my_string[-3:-1]) # Prints "bc"
print(my_string[-2:]) # Prints "cd"
print(my_string[:-2]) # Prints "ab"
```

We can also use a step value in slicing. The step value determines how many characters are skipped between each character that is included in the slice. The step value can be positive or negative and defaults to 1.

```py
my_string = "abcd"
print(my_string[0:4:2]) # Prints "ac"
print(my_string[1:4:2]) # Prints "bd"
print(my_string[0:4:3]) # Prints "ad"
print(my_string[3:0:-1]) # Prints "dcb"
print(my_string[::-1]) # Prints "dcba"
```

#### String Methods

Strings have a number of useful methods that can be used to manipulate them. We can call a method on a string by using the syntax `string.method()`. For example, the `upper()` method converts the string to uppercase.

```py
my_string = "Hello World"
print(my_string.upper()) # Prints "HELLO WORLD"
```

_Recall: A method is a function that is used in the context of a specific object_

We can also call methods on a string literal. For example, the `upper()` method can be called on a string literal.

```py
print("Hello World".upper()) # Prints "HELLO WORLD"
```

_A string literal is a string that is not stored in a variable but is instead written in quotes._

We can also call methods on the result of a function. For example, the `upper()` method can be called on the result of the `input()` function.

```py
name = input("Enter your name: ").upper()
print(name) # Prints the user's name in uppercase
```

Methods can also be chained together. For example, the `strip()` method can be chained with the `lower()` method.

```py
my_string = " Hello World "
print(my_string.strip().lower()) # Prints "hello world"
```

Methods can also take arguments. For example, the `replace()` method takes two arguments, the first is the character to replace and the second is the character to replace it with.

```py
my_string = "Hello World"
print(my_string.replace("o", "a")) # Prints "Hella Warld"
```

#### Useful Methods

Here is a list of a few useful string methods.

| Method              | Description                                                |
| ------------------- | ---------------------------------------------------------- |
| `upper()`           | Converts the string to uppercase                           |
| `lower()`           | Converts the string to lowercase                           |
| `capitalize()`      | Capitalizes the first character of the string              |
| `title()`           | Capitalizes the first character of each word in the string |
| `strip()`           | Removes whitespace from the start and end of the string    |
| `lstrip()`          | Removes whitespace from the start of the string            |
| `rstrip()`          | Removes whitespace from the end of the string              |
| `replace(old, new)` | Replaces all instances of `old` with `new`                 |
| `split()`           | Splits the string into a list of substrings                |
| `join(list)`        | Joins the elements of a list into a string                 |
