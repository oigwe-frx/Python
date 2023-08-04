# Boolean Expressions

A boolean expression is a statement that can either be True or False.


# Rational Operations: Equat and Not Equat

Relational operators compare two items and return either True or False. For this reason, you will sometimes hear them called comparators.
The two relational operators we’ll cover first are:

Equals: ```==```
Not equals: ```!=```

```
1 == 1     # True
 
2 != 4     # True
 
3 == 5     # False
 
'7' == 7   # False
```

Why is the last statement false? The '' marks in '7' make it a string, which is different from the integer value 7, so they are not equal. When using relational operators it is important to always be mindful of type.


# Boolean Variables

True and False are the only bool types, and any variable that is assigned one of these values is called a boolean variable.

Boolean variables can be created in several ways. The easiest way is to simply assign True or False to a variable:

```
set_to_true = True
set_to_false = False
```
 
You can also set a variable equal to a boolean expression.

```
bool_one = 5 != 7 
bool_two = 1 + 1 != 2
bool_three = 3 * 3 == 9
```
 
These variables now contain boolean values, so when you reference them they will only return the True or False values of the expression they were assigned.

```
print(bool_one)    # True
 
print(bool_two)    # False
 
print(bool_three)  # True
```

# If Statement

```
if is_raining:
  print("bring an umbrella")
```
You’ll notice that instead of “then” we have a colon, ```:```. 
That tells the computer that what’s coming next is what should be executed if the condition is met.

```
def dave_check(user_name):
  if user_name == "Dave":
    return "Get off my computer Dave!"
  if user_name == "angela_catlady_87":
    return "I know it is you Dave! Go away!"
```

# Relational Operators II


# Boolean Operations: and
# Boolean Operators: or
# Boolean Operators: not
# Else Statement
# Else If Statements
