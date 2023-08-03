# Comments
Python interprets anything after a # as a comment.

# Print
```print()``` function is used to tell a computer to talk. The message to be printed should be surrounded by quotes:

```
# from Mary Shelley's Frankenstein
print("There is something at work in my soul, which I do not understand.")
```

# Strings
In Python a string is either surrounded by double quotes ("Hello world") or single quotes ('Hello world'). It doesn’t matter which kind you use, just be consistent.
```print("Osita")```
```print('Osita')```

# Variables

```
message_string = "Hello there"
# Prints "Hello there"
print(message_string)
```

- Variables can’t have spaces or symbols in their names other than an underscore (_).
- They can’t begin with numbers but they can have numbers after the first letter (e.g., cool_variable_5 is OK).

# Errors

## SyntaxError
means there is something wrong with the way your program is written — punctuation that does not belong, a command where it is not expected, or a missing parenthesis can all trigger a SyntaxError.
> - Ex:  if you open a string with a single quote and end it with double quotes. 

##ameError
occurs when the Python interpreter sees a word it does not recognize. Code that contains something that looks like a variable but was never defined will throw a NameError.
> - Ex:  you try to print a single word string but fail to put any quotes around it. Python expects the word of your string to be defined elsewhere but can’t find where it’s defined. Add quotes to either side of the string to squash this bug.


# Numbers
Python has a few numeric data types. 

## An integer$$
```int``
Is a whole number. It has no decimal point and contains all counting numbers (1, 2, 3, …) as well as their negative counterparts and the number 0. If you were counting the number of people in a room, the number of jellybeans in a jar, or the number of keys on a keyboard you would likely use an integer.

## A floating-point number,
```float``` 
Is a decimal number. It can be used to represent fractional quantities as well as precise measurements. If you were measuring the length of your bedroom wall, calculating the average test score of a seventh-grade class, or storing a baseball player’s batting average for the 1998 season you would likely use a float.

Numbers can be assigned to variables or used literally in a program:

```
an_int = 2
a_float = 2.1
 
print(an_int + 3)
# Output: 5
```

