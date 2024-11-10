# Python Data Types

## Built-in Data Types
In programming, data type is an important concept.

Variables can store data of different types, and different types can do different things.

Python has the following data types built-in by default, in these categories:

Text Type:	str <br>
Numeric Types:	int, float, complex
Sequence Types:	list, tuple, range<br>
Mapping Type:	dict
Set Types:	set, frozenset
Boolean Type:	bool
Binary Types:	bytes, bytearray, memoryview
None Type:	NoneType

### Setting the Data Type
In Python, the data type is set when you assign a value to a variable:

Example	Data Type	
x = "Hello World" -	str\	
x = 20 -	int\	
x = 20.5	- float	
x = 1j -	complex	
x = ["apple", "banana", "cherry"]	- list	
x = ("apple", "banana", "cherry")	- tuple	
x = range(6)	- range	
x = {"name" : "John", "age" : 36} -	dict	
x = {"apple", "banana", "cherry"}	- set	
x = frozenset({"apple", "banana", "cherry"})	- frozenset	
x = True	- bool	
x = b"Hello"	- bytes	
x = bytearray(5)	- bytearray	
x = memoryview(bytes(5))	- memoryview	
x = None	- NoneType	

## Python Numbers
There are three numeric types in Python:

- **int**
- **float**
- **complex**

Example
x = 1    # int
y = 2.8  # float
z = 1j   # complex

Int
Int, or integer, is a whole number, positive or negative, without decimals, of unlimited length.

Float
Float, or "floating point number" is a number, positive or negative, containing one or more decimals.

Complex
Complex numbers are written with a "j" as the imaginary part:


Random Number
Python does not have a random() function to make a random number, but Python has a built-in module called random that can be used to make random numbers:
ex- 
import random

print(random.randrange(1, 10))
