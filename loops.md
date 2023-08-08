# For Loops

```
for <temporary variable> in <collection>:
  <action>
```

```
ingredients = ["milk", "sugar", "vanilla extract", "dough", "chocolate"]
 
for ingredient in ingredients:
  print(ingredient)
 ```

__NOTE:__ If we ever forget to indent, we’ll get an IndentationError or unexpected behavior.


# Using Range

Often we won’t be iterating through a specific list (or any collection), but rather only want to perform a certain action multiple times.

```
for <temporary variable> in <list of length 6>:
  print("Learning Loops!")
```

To create arbitrary collections of any length, we can pair our for loops with the Python built-in function range().
An example of how the range() function works, this code generates a collection of 6 integer elements from 0 to 5:

```
six_steps = range(6)
 
# six_steps is now a collection with 6 elements:
# 0, 1, 2, 3, 4, 5
```

```
for temp in range(6):
  print("Learning Loops!") //  Learning Loops!
Learning Loops!
Learning Loops!
Learning Loops!
Learning Loops!
Learning Loops!
```

# While Loops

A while loop performs a set of instructions as long as a given condition is true.

```
while <conditional statement>:
  <action>
```

```
count = 0
while count <= 3:
  # Loop Body
  print(count)
  count += 1
```

## Lists

```length = len(ingredients)
index = 0
 
while index < length:
  print(ingredients[index])
  index += 1
```


