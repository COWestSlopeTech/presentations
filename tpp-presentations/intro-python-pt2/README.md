## Introduction to Python
### Iteration, Functions, Libraries, and more
Jeremy Cerise and the Roaring Fork Technologists

### Ground Rules
Before we get started...


	* We're here to support each other

	* We're here to learn from each other

	* We're here to teach each other

	* We're here to encourage each other


But most importantly

There is no "stupid" in this room

### What we learned last time


	* Basic Syntax

	* Data types

	* Variables

	* Basic data structures (List, Dictionary)

	* Basic Arithmetic (+, -, /,  *)

	* Conditionals (If/else)

### What we'll learn this time

	* Iteration 

	* Functions

	* Variable scope

	* Libraries

	* Putting it all together

### Tools
IDEs

An IDE is an Integrated Development Environment, and they can greatly simplify the process of writing software.

***In order to use these, you will need a python installation on your computer***

		* Jetbrains Pycharm: https://www.jetbrains.com/pycharm/

		* Atom: https://atom.io/

		* Visual Studio Code: https://code.visualstudio.com/


None of these are necessary, and repl.it (which we used last time) is totally fine, if you want to use that.

### Iteration - The while loop

Iteration is repeating an action over and over and over until a condition is met.

```
count = 0
while count <= 10:
    print("Count is equal to: " + count)
    count = count + 1
```


What should the output be?

```
Count is equal to: 1
Count is equal to: 2
Count is equal to: 3
Count is equal to: 4
Count is equal to: 5
Count is equal to: 6
Count is equal to: 7
Count is equal to: 8
Count is equal to: 9
Count is equal to: 10
```

### Iteration - The for loop

A for loop will iterate a set, or known, number of times. For loops can also iterate over elements of data structures (lists, dictionaries)


```
for count in [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]:
    print("Count is equal to: " + count)
```


What should the output be?


Another way to write the above:

```
for i in range(1, 10):
    print("Count is equal to: " + i
```

### Functions
A function is a block of code that only executes when called.


Functions can be passed data, known as parameters.


Functions can return data.


Lets look at an example:


```
def add_two_numbers(x, y):
    new_value = x + y
    return new_value

add_two_numbers(1, 2)

3

```

### Functions (Cont.)

A function can call another function


```
def print_greeting(name):
    addition_result = add_two_numbers(1, 2)
    print("Hello, " + name + ", 1 + 2 is " + addition_result")

print_greeting("Jeremy")

Hello, Jeremy, 1 + 2 is 3
```

### Functions and Variable Scope 
Variables that are defined inside of a function can only be accessed inside that function.

```
def add_two_numbers(x, y):
    return x + y

add_two_numbers(1, 2)

3

print(x)

Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'x' is not defined
```

### Repl.it Putting it together example

https://repl.it/@JeremyCerise/GitHubPython-API-Example
