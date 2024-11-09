
**python syntax**
## Execute Python Syntax

Python syntax can be executed by writing directly in the Command Line
print("Hello, World!")
Hello, World!

## Python Indentation

Indentation refers to the spaces at the beginning of a code line.

Where in other programming languages the indentation in code is for readability only, the indentation in Python is very important.

Example
if 5 > 2:
  print("Five is greater than two!")

## Python Variables

In Python, variables are created when you assign a value to it:

Example 
x = 5
y = "Hello, World!"

**Python has no command for declaring a variable.**

## Comments
Comments start with a #, and Python will render the rest of the line as a comment:

Example 
#This is a comment.
print("Hello, World!")

## Multiline Comments

Example
"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")

# Python Variables

### Variables 
Variables are containers for storing data values.

#### Casting
If you want to specify the data type of a variable, this can be done with casting.

Example
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0

## How to get the type of variable
x = 5
y = "John"
print(type(x))
print(type(y))

### Single or Double Quotes?
String variables can be declared either by using single or double quotes: the output will be tehh same in double and single quote

ex - x = "John"
// is the same as
x = 'John'

## Variable Names

A variable can have a short name (like x and y) or a more descriptive name (age, carname, total_volume). Rules for Python variables:\
A variable name must start with a letter or the underscore character\
A variable name cannot start with a number\
A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )\
Variable names are case-sensitive (age, Age and AGE are three different variables)\
A variable name cannot be any of the Python keywords.\

ex- myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"

## Multi Words Variable Names
Variable names with more than one word can be difficult to read.

There are several techniques you can use to make them more readable:

### Camel Case
Each word, except the first, starts with a capital letter: 
myVariableName = "John"

### Pascal Case
Each word starts with a capital letter:
MyVariableName = "John"

### Snake Case
Each word is separated by an underscore character:
my_variable_name = "John"

## Many Values to Multiple Variables
Python allows you to assign values to multiple variables in one line:
ex-
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)

### One Value to Multiple Variables
And you can assign the same value to multiple variables in one line:
ex-
x = y = z = "Orange"
print(x)
print(y)
print(z)

## Unpack a Collection
If you have a collection of values in a list, tuple etc. Python allows you to extract the values into variables. This is called unpacking.
ex-
fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)

# Question - What is a correct syntax to add the value 'Hello World', to 3 variables in one statement?
ans - x = y = z = 'Hello World'

# Output Variables
The Python print() function is often used to output variables.
ex - 
x = "Python is awesome"
print(x)

In the print() function, you output multiple variables, separated by a comma:
ex- x = "Python"
y = "is"
z = "awesome"
print(x, y, z)

output - Python is awesome

**You can also use the + operator to output multiple variables:**
ex- x = "Python "
y = "is "
z = "awesome"
print(x + y + z)

output - Python is awesome
**Notice the space character after "Python " and "is ", without them the result would be "Pythonisawesome".**

# Question -- Consider the following code: print('Hello', 'World') What will be the printed result?
ans - Hello World

## Global Variables

Variables that are created outside of a function (as in all of the examples in the previous pages) are known as global variables.
Global variables can be used by everyone, both inside of functions and outside.

ex - Create a variable outside of a function, and use it inside the function
x = "awesome"
def myfunc():
  print("Python is " + x)

myfunc()
output - 
x = "awesome"
​
def myfunc():
  print("Python is " + x)
​
myfunc()
​output - Python is awesome

Ex - 
x = "awesome"
def myfunc():
  x = "fantastic"
  print("Python is " + x)
myfunc()
print("Python is " + x)
output - Python is fantastic
Python is awesome

## The global Keyword
Normally, when you create a variable inside a function, that variable is local, and can only be used inside that function.

To create a global variable inside a function, you can use the global keyword.
ex- 
x = "awesome"
def myfunc():
  global x
  x = "fantastic"
myfunc()
print("Python is " + x)
output - Python is fantastic

