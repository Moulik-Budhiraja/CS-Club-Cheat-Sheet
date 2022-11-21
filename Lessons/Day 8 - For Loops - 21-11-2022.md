# For Loops

#### 21-11-2022

---

[Back to Table of Contents](/README.md)

## In this lesson

-   [What is a For Loop?](#what-is-a-for-loop)
-   [Syntax](#syntax)
    -   [Example](#example)
    -   [Breakdown](#breakdown)
-   [Range](#range)
-   [Enumerate](#enumerate)
-   [Break and Continue](#break-and-continue)

### What is a For Loop?

A for loop is used to iterate over a sequence. So far we've looked at two types of sequences: strings and lists. We can use a for loop to iterate over each character in a string or each item in a list.

### Syntax

The syntax for a for loop is:

```py
for item in sequence:
    # Do something with item
```

#### Example

For example we can use a for loop to double each item in a list:

```py
my_list = [1, 2, 3]

doubled_list = []

for item in my_list:
    doubled_list.append(item * 2)
```

#### Breakdown

-   `for item in my_list:` - This is the for loop. We can call the variable `item` anything we want. It's just a variable that we can use to access the current item in the sequence. In this case we're iterating over a list so we can call it `item`. If we were iterating over a string we could call it `char`.

-   `doubled_list.append(item * 2)` - This is the code that we want to run for each item in the sequence. In this case we're multiplying the item by 2 and appending it to the `doubled_list`.

### Range

The `range()` function is used to generate a sequence of numbers. It takes 3 parameters:

-   `start` - The number to start from. This is optional and defaults to 0.
-   `stop` - The number to stop at. This is required.
-   `step` - The amount to increment by. This is optional and defaults to 1.

```py
for i in range(5):
    print(i)
```

```py
for i in range(1, 11):
    print(i)
```

This will print the numbers 1 to 10.

### Enumerate

Sometimes we want to access the index of each item in a sequence along with the item itself. One way to do this is to loop over a range of the length of the sequence and use that to access the items.

```py
my_list = [1, 2, 3]

for i in range(len(my_list)):
    item = my_list[i]

    print(i, item)
```

But Python has a built-in function called `enumerate()` that does this for us. It returns a tuple containing the index and item. We can break up the tuple into two variables using tuple unpacking.

```py
my_list = [1, 2, 3]

for index, item in enumerate(my_list):
    print(index, item)
```

### Break and Continue

We can use the `break` keyword to exit a for loop early. For example if we wanted to find the first even number in a list we could use a for loop and break once we find it.

```py
my_list = [1, 3, 5, 4, 2]

for item in my_list:
    if item % 2 == 0:
        print(item)
        break
```

We can use the `continue` keyword to skip the current iteration of the loop and continue to the next one. For example if we wanted to print all the odd numbers in a list we could use a for loop and continue if the number is even.

```py
my_list = [1, 3, 5, 4, 2]

for item in my_list:
    if item % 2 == 0:
        continue
    print(item)
```
