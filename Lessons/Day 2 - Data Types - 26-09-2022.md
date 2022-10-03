# Data Types

#### 26-09-2022

---

[Back to Table of Contents](/README.md)

### Basic Data Types

There are 4 basic data types in Python:

-   Strings
-   Integers
-   Floats
-   Booleans

#### Strings

Strings are used to store text. Strings are surrounded by either single quotes or double quotes.

```py
x = "This is a string"
y = 'This is also a string'
```

#### Integers

Integers are used to store whole numbers. Integers can be positive or negative.

```py
x = 5
y = -5
z = 0
```

#### Floats

Floats are used to store decimal numbers. Floats can be positive or negative.

```py
w = 5.0
x = 5.5
y = -5.5
z = 0.0
```

#### Booleans

Booleans are used to store true or false values. Booleans are used in if statements.

```py
x = True
y = False
```

### Type Conversion

We can convert between data types using the following functions:

-   `str()` - Converts to a string
-   `int()` - Converts to an integer
-   `float()` - Converts to a float
-   `bool()` - Converts to a boolean

```py
x = 5
y = 5.5
z = "5"

x = str(x) # x is now "5"
y = int(y) # y is now 5
z = float(z) # z is now 5.0
```

### Checking Type

We can check the type of a variable using the `type()` function.

```py
x = 5
y = 5.5
z = "5"

print(type(x)) # <class 'int'>
print(type(y)) # <class 'float'>
print(type(z)) # <class 'str'>
```

### Math Operators

We can use the following operators to do math:

| Operator | Function         |
| -------- | ---------------- |
| `+`      | Addition         |
| `-`      | Subtraction      |
| `*`      | Multiplication   |
| `/`      | Division         |
| `**`     | Exponent         |
| `%`      | Modulus          |
| `//`     | Integer Division |

```py
x = 5
y = 5.5
z = 15

print(x + y) # 10.5
print(x - y) # -0.5
print(x * y) # 27.5
print(z / x) # 3.0
print(z ** x) # 759375
print(z % x) # 0
print(z // x) # 3
```

### Control Flow

Control flow is used to control the flow of a program. We can use control flow to make decisions in our program with the `if`, `elif` and `else` keywords.

```py
num = int(input("Enter a number: "))

if num > 5:
    print("Input is bigger then 5")
elif num < 5:
    print("Input is smaller then 5")
else:
    print("Input is equal to 5")
```

```
Enter a number: 5
>>> Input is equal to 5
```

```
Enter a number: 4
>>> Input is smaller then 5
```

```
Enter a number: 6
>>> Input is bigger then 5
```
