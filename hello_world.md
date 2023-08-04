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

Numbers can be assigned to variables ```a_float = 2.1
``` or used literally ```2.1``` in a program:

```
an_int = 2
a_float = 2.1
 
print(an_int + 3)
# Output: 5
```

# Calculations
Python performs the arithmetic operations of addition, subtraction, multiplication, and division with +, -, *, and /.

```
# Prints "500"
print(573 - 74 + 1)
 
# Prints "50"
print(25 * 2)
 
# Prints "2.0"
print(10 / 5)
```
Python converts all ints to floats before performing division. In older versions of Python (2.7 and earlier) this conversion did not happen, and integer division would always round down to the nearest integer.

Division can throw its own special error: 
__ZeroDivisionError:__ Python will raise this error when attempting to divide by 0.

# Changing Numbers

Variables that are assigned numeric values can be treated the same as the numbers themselves. 
- Two variables can be added together, divided by 2, and multiplied by a third variable without Python distinguishing between the variables and literals (like the number 2 in this example).
- Performing arithmetic on variables does not change the variable — you can only update a variable using the = sign.

```
coffee_price = 1.50
number_of_coffees = 4
 
# Prints "6.0"
print(coffee_price * number_of_coffees)
# Prints "1.5"
print(coffee_price)
# Prints "4"
print(number_of_coffees)
 
# Updating the price 
coffee_price = 2.00
 
# Prints "8.0"
print(coffee_price * number_of_coffees)
# Prints "2.0"
print(coffee_price)
# Prints "4"
print(number_of_coffees)
```

# Exponents

Python can also perform exponentiation. 

Since this operation is so related to multiplication, we use the notation **.

```
# 2 to the 10th power, or 1024
print(2 ** 10)
 
# 8 squared, or 64
print(8 ** 2)
 
# 9 * 9 * 9, 9 cubed, or 729
print(9 ** 3)
 
# We can even perform fractional exponents
# 4 to the half power, or 2
print(4 ** 0.5)
```

# Modulo

Python offers a companion to the division operator called the modulo operator.

The modulo operator is indicated by % and gives the remainder of a division calculation. If the number is divisible, then the result of the modulo operator will be 0.

```
# Prints 4 because 29 / 5 is 5 with a remainder of 4
print(29 % 5)
 
# Prints 2 because 32 / 3 is 10 with a remainder of 2
print(32 % 3)
 
# Modulo by 2 returns 0 for even numbers and 1 for odd numbers
# Prints 0
print(44 % 2)
```

# Concatenation

The + operator doesn’t just add two numbers, it can also “add” two strings! 

The process of combining two strings is called string concatenation. 

Performing string concatenation creates a brand new string comprised of the first string’s contents followed by the second string’s contents (without any added space in-between).

```
greeting_text = "Hey there!"
question_text = "How are you doing?"
full_text = greeting_text + question_text
 
# Prints "Hey there!How are you doing?"
print(full_text)
```

# Plus Equals

When you have a number saved in a variable and want to add to the current value of the variable, you can use the += (plus-equals) operator.

```
# First we have a variable with a number saved
number_of_miles_hiked = 12
 
# Then we need to update that variable
# Let's say we hike another two miles today
number_of_miles_hiked += 2
 
# The new value is the old value
# Plus the number after the plus-equals
print(number_of_miles_hiked)
# Prints 14
```

The plus-equals operator also can be used for string concatenation, like so:

```
hike_caption = "What an amazing time to walk through nature!"
 
# Almost forgot the hashtags!
hike_caption += " #nofilter"
hike_caption += " #blessed"
```

# Multi-line Strings

Python strings are very flexible, but if we try to create a string that occupies multiple lines we find ourselves face-to-face with a SyntaxError. 

Python offers a solution: multi-line strings. By using three quote-marks (""" or ''') instead of one, we tell the program that the string doesn’t end until the next triple-quote. 

This method is useful if the string being defined contains a lot of quotation marks and we want to be sure we don’t close it prematurely.

```
leaves_of_grass = """
Poets to come! orators, singers, musicians to come!
Not to-day is to justify me and answer what I am for,
But you, a new brood, native, athletic, continental, greater than
  before known,
Arouse! for you must justify me.
"""
```

# User Input

Another way to assign a value to a variable is through user input.

The input() function requires a prompt message, which it will print out for the user before they enter the new information. For example:
```
likes_snakes = input("Do you like snakes? ")

# The variable likes_snakes would be assigned a value of the user’s answer.

```

Once you have that information stored as a variable you can use it to simulate interaction:

```
>>> favorite_fruit = input("What is your favorite fruit? ")
What is your favorite fruit? mango
 
>>> print("Oh cool! I like " + favorite_fruit + " too, but I think my favorite fruit is apple.")
Oh cool! I like mango too, but I think my favorite fruit is apple.
 
```
