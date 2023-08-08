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

# Lists

length = len(ingredients)

```
index = 0
 
while index < length:
  print(ingredients[index])
  index += 1
```

# Breaks

```
items_on_sale = ["blue shirt", "striped socks", "knit dress", "red headband", "dinosaur onesie"]
 
print("Checking the sale list!")
 
for item in items_on_sale:
  print(item)
  if item == "knit dress":
    break
 
print("End of search!")
```

When the program hits a break statement it immediately terminates a loop. For example:


# Continue

While the break control statement will come in handy, there are other situations where we don’t want to end the loop entirely. What if we only want to skip the current iteration of the loop?

```
big_number_list = [1, 2, -1, 4, -5, 5, 2, -9]

for i in big_number_list:
  if i <= 0: // Goal to print out only positive numbers
    continue
  print(i)  // 1 2 4 5 2 
 ```

```
ages = [12, 38, 34, 26, 21, 19, 67, 41, 17]

for age in ages:
  if age < 21:
    continue
  else: 
    print(age)
```

# Nested Loops

```
# Loop through each sublist
for team in project_teams:

  # Loop elements in each sublist
  for student in team:
    print(student)

```

# List Comprehension

```
grades = [90, 88, 62, 76, 74, 89, 48, 57]

scaled_grades = [ grade + 10 for grade in grades]

print(scaled_grades)
```

```
numbers = [2, -1, 79, 33, -45]
negative_doubled = [num * 2 for num in numbers if num < 0]
print(negative_doubled)
```

```
numbers = [2, -1, 79, 33, -45]
doubled = [num * 2 if num < 0 else num * 3 for num in numbers ]
print(doubled)
```

