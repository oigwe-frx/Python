# What is a List? - an array

In programming, it is common to want to work with collections of data. In Python, a list is one of the many built-in data structures that allows us to work with a collection of data in sequential order.

```
heights = [61, 70, 67, 64]
```

# What can a List contain?

Lists can contain any data type in Python! For example, this list contains a string, integer, boolean, and float.


```
mixed_list_common = ["Mia", 27, False, 0.5]
```

# Empty Lists

A list doesn’t have to contain anything. You can create an empty list like this:

```
my_empty_list = []
```

# List Methods

For lists, methods will follow the form of ___list_name.method()___. S
ome methods will require an input value that will go between the parenthesis of the method ( ).



## Append

We can add a single element to a list using the ___.append()___ Python method. 
On a list that already has elements, our new element is added to the end of the list:

```
garden = []

garden.append("Tomatoes")
 
print(garden) // ['Tomatoes']
```

### Plus (+)

When we want to add multiple items to a list, we can use + to combine two lists (this is also known as concatenation).

```
items_sold = ["cake", "cookie", "bread"]
items_sold_new = items_sold + ["biscuit", "tart"]
print(items_sold_new) // ['cake', 'cookie', 'bread', 'biscuit', 'tart']
```

## Accessing List Elements

In Python, we call the location of an element in a list its index.

Python lists are zero-indexed. This means that the first element in a list has index 0, rather than 1.

```
calls = ["Juan", "Zofia", "Amare", "Ezio", "Ananya"]
print(calls[2]) // Amare
```

## Accessing List Elements: Negative Index

What if we want to select the last element of a list?

We can use the index -1 to select the last item of a list, even when we don’t know how many elements are in a list.

```
pancake_recipe = ["eggs", "flour", "butter", "milk", "sugar", "love"]
print(pancake_recipe[-1]) //love
aka
print(pancake_recipe[5])

```

## Modifying List Elements

To change a value in a list, reassign the value using the specific index.

```
garden[2] = "Strawberries"
 
print(garden) // ["Tomatoes", "Green Beans", "Strawberries", "Grapes"]

garden[-1] = "Raspberries"
 
print(garden) // ["Tomatoes", "Green Beans", "Strawberries", "Raspberries"]

```

## Remove

We can remove elements in a list using the ___.remove()___ Python method.

```
shopping_line = ["Cole", "Kip", "Chris", "Sylvana"]

shopping_line.remove("Chris")
 
print(shopping_line) // ["Cole", "Kip", "Sylvana"]

```

We can also use .remove() on a list that has duplicate elements.

Only the first instance of the matching element is removed:

```
shopping_line = ["Cole", "Kip", "Chris", "Sylvana", "Chris"]
 
# Remove an element
shopping_line.remove("Chris")
print(shopping_line) // ["Cole", "Kip", "Sylvana", "Chris"]
```

# Two-Dimensional (2D) Lists

Lists can contain other lists! We will commonly refer to these as two-dimensional (2D) lists.

```
heights = [["Jenny", 61], ["Alexus", 70], ["Sam", 67], ["Grace", 64]]
```

We will often find that a two-dimensional list is a very good structure for representing grids such as games like tic-tac-toe.

tic_tac_toe = [
            ["X","O","X"], 
            ["O","X","O"], 
            ["O","O","X"]
]

## Accessing 2D Lists

Two-dimensional lists can be accessed similarly to their one-dimensional counterpart. Instead of providing a single pair of brackets [ ] we will use an additional set for each dimension past the first.

```
#Access the sublist at index 0, and then access the 1st index of that sublist.

heights = [["Noelle", 61], ["Ali", 70], ["Sam", 67]]
noelles_height = heights[0][1] 
print(noelles_height) //61
```

## Modifying 2D Lists

To change a value in a two-dimensional list, reassign the value using the specific index.

```
class_name_hobbies = [["Jenny", "Breakdancing"], ["Alexus", "Photography"], ["Grace", "Soccer"]]

# The list of Jenny is at index 0. The hobby is at index 1. 
class_name_hobbies[0][1] = "Meditation"
print(class_name_hobbies) // [["Jenny", "Meditation"], ["Alexus", "Photography"], ["Grace", "Soccer"]]
```

Negative indices will work as well.

```
# The list of Grace is the last entry. The hobby is the last element. 
class_name_hobbies[-1][-1] = "Football"
print(class_name_hobbies) //[["Jenny", "Meditation"], ["Alexus", "Photography"], ["Grace", "Football"]]
```


# Methods

## Insert

The Python list method ___.insert()___ allows us to add an element to a specific index in a list.

The .insert() method expects two inputs, the first being a numerical index, followed by any value as the second input:

- The index you want to insert into.
- The element you want to insert at the specified index.

The .insert() method will handle shifting over elements and can be used with negative indices.

```
store_line = ["Karla", "Maxium", "Martim", "Isabella"]
store_line.insert(2, "Vikor") //  ['Karla', 'Maxium', 'Vikor', 'Martim', 'Isabella']
```


## Pop

Python gives us a method to remove elements at a specific index using a method called __.pop()__.

The .pop() method takes an optional single input:

- The index for the element you want to remove.
- The method can be called without a specific index. Using .pop() without an index will remove whatever the last element of the list is. In our case "Clowns 101" gets removed.
- .pop() is unique in that it will return the value that was removed. If we wanted to know what element was deleted, simply assign a variable to the call of the .pop() method. In this case, we assigned it to removed_element.
- ___Note:___ Passing in an index that does not exist or calling .pop() on an empty list will both result in an IndexError.



```
cs_topics = ["Python", "Data Structures", "Balloon Making", "Algorithms", "Clowns 101"]
cs_topics.pop(2)
print(cs_topics) //['Python', 'Data Structures', 'Algorithms']
```

## Range

The function __range()__ takes a single input, and generates numbers starting at 0 and ending at the number __before__ the input.

The range() function is unique in that it creates a range object. It is not a typical list like the ones we have been working with.

In order to use this object as a list, we have to first convert it using another built-in function called __list()__

```
zero_to_seven = range(7)
print(list(zero_to_seven)) // [0, 1, 2, 3, 4, 5, 6]

```

By default, range() creates a list starting at 0. However, if we call range() with two inputs, we can create a list that starts at a different number.

```
my_list = range(2, 9)
print(list(my_list)) //[2, 3, 4, 5, 6, 7, 8]
```
If we use a third input, we can create a list that “skips” numbers.

For example, range(2, 9, 2) will give us a list where each number is 2 greater than the previous number:

```
my_range2 = range(2, 9, 2)
print(list(my_range2)) // [2, 4, 6, 8]
```
We can skip as many numbers as we want!

```
my_range3 = range(1, 100, 10)
print(list(my_range3)) // [1, 11, 21, 31, 41, 51, 61, 71, 81, 91]

Our list stops at 91 because the next number in the sequence would be 101, which is greater than or equal to 100 (our stopping point).

``` 

## Length

When we apply ___len()___ to a list, we get the number of elements in that list:

```
my_list = [1, 2, 3, 4, 5]
 
print(len(my_list)) // 5
```


## Slicing Lists 

In Python, often we want to extract only a portion of a list. Dividing a list in such a manner is referred to as slicing.

We can do this using the following syntax: ```list[start:end]```, where:

- Inclusive - start is the index of the first element that we want to include in our selection.
- Exclusive - end is the index of one more than the last index that we want to include.

```
letters = ["a", "b", "c", "d", "e", "f", "g"]
sliced_list = letters[1:6]
print(sliced_list) // ["b", "c", "d", "e", "f"]
```
If we want to select the first n elements of a list, we could use the following code:

```
fruits[:n]
print(fruits[:3])
```
We can do something similar when we want to slice the last n elements in a list:

```
fruits[-n:] //Inclusive
print(fruits[-2:]) // This code slices from the element at index -2 up through the last index.
```

## Counting in a List

Suppose we have a list called letters that represents the letters in the word “Mississippi”:

```letters = ["m", "i", "s", "s", "i", "s", "s", "i", "p", "p", "i"]```

If we want to know how many times ```i``` appears in this word, we can use the list method called __.count()__:

```
num_i = letters.count("i")
print(num_i) //4
```
Since .count() returns a value, we can assign it to a variable to use it.

We can even use .count() to count element appearances in a two-dimensional list.

```
number_collection = [[100, 200], [100, 200], [475, 29], [34, 34]]

# How often the sublist [100, 200] appears:

num_pairs = number_collection.count([100, 200])
print(num_pairs) //2
```


## Sorting Lists

Often, we will want to sort a list in either numerical (1, 2, 3, …) or alphabetical (a, b, c, …) order.

We can sort a list using the method ___.sort()___.

```
names = ["Xander", "Buffy", "Angel", "Willow", "Giles"]
names.sort()
print(names) // ['Angel', 'Buffy', 'Giles', 'Willow', 'Xander']
```

.sort() also provides us the option to go in reverse. Instead of sorting in ascending order like we just saw, we can do so in descending order.

```
names = ["Xander", "Buffy", "Angel", "Willow", "Giles"]
names.sort(reverse=True)
print(names) // ['Xander', 'Willow', 'Giles', 'Buffy', 'Angel']
```

__Note:__ The .sort() method does not return any value and thus does not need to be assigned to a variable since it modifies the list directly. If we do assign the result of the method, it would assign the value of None to the variable.






 









































 






 


