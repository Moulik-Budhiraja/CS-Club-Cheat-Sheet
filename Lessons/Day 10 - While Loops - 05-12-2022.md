# While Loops

#### 05-12-2022

---

[Back to Table of Contents](/README.md)

## In this lesson

-   [What is a Wile Loop?](#what-is-a-while-loop)
-   [Syntax](#syntax)
    -   [Example](#example)
    -   [Breakdown](#breakdown)
-   [Break and Continue](#break-and-continue)

### What is a While Loop?

A while loop is used to repeat a block of code while a condition is true.

### Syntax

The syntax for a while loop is:

```py
while condition:
    # Do something
```

#### Example

For example we can use a while loop to print the numbers 1 to 10:

```py
i = 1

while i <= 10:
    print(i)
    i += 1
```

#### Breakdown

-   `while i <= 10:` - This is the while loop. We can call the variable `i` anything we want. It's just a variable that we can use to keep track of the current number. In this case we're starting at 1 so we can call it `i`.
-   `print(i)` - This is the code that we want to run while the condition is true. In this case we're printing the current number.
-   `i += 1` - This is the code that we want to run after the code block has finished. In this case we're incrementing `i` by 1.

### Break and Continue

We can use the `break` and `continue` keywords to control the flow of a loop.

-   `break` - This will stop the loop completely.
-   `continue` - This will stop the current iteration and continue to the next one.

For example we can use a while loop to print the numbers 1 to 10 but skip the number 5:

```py
i = 1

while i <= 10:
    if i == 5:
        i += 1
        continue

    print(i)
    i += 1
```
