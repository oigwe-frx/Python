# Defining a Function

```
def trip_welcome():
  print("Welcome to Tripcademy!") 
  print("Let's get you to your destination.")
```

- The def keyword indicates the beginning of a function (also known as a function header). The function header is followed by a name in snake_case format that describes the task the function performs. It’s best practice to give your functions a descriptive yet concise name.

- Following the function name is a pair of parenthesis ( ) that can hold input values known as parameters (more on parameters later in the lesson!). In this example function, we have no parameters.

- A colon : to mark the end of the function header.

- Lastly, we have one or more valid python statements that make up the function body (where we have our python comment).

## Positional Arguments

```
def calculate_taxi_price(miles_to_travel, rate, discount):
  print(miles_to_travel * rate - discount )
```

```
# 100 is miles_to_travel
# 10 is rate
# 5 is discount
calculate_taxi_price(100, 10, 5)
```

## Keyword Arguments

Explicitly refer to what each argument is assigned to in the function call. Notice in the code example below that the arguments do not follow the same order as defined in the function declaration.

```
calculate_taxi_price(rate=0.5, discount=10, miles_to_travel=100)
```

## Default aka same as in javascript

```
def calculate_taxi_price(miles_to_travel, rate, discount = 10):
  print(miles_to_travel * rate - discount )
```
