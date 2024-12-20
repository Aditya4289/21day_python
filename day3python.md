# Python Casting

## Specify a Variable Type

There may be times when you want to specify a type on to a variable. This can be done with casting. Python is an object-orientated language, and as such it uses classes to define data types, including its primitive types.

Casting in python is therefore done using constructor functions:

- int() - constructs an integer number from an integer literal, a float literal (by removing all decimals), or a string literal (providing the string represents a whole number)
- float() - constructs a float number from an integer literal, a float literal or a string literal (providing the string represents a float or an integer)
- str() - constructs a string from a wide variety of data types, including strings, integer literals and float literals

## Python Strings

### Strings

Strings in python are surrounded by either single quotation marks, or double quotation marks.

'hello' is the same as "hello".

You can display a string literal with the print() function

### Quotes Inside Quotes

You can use quotes inside a string, as long as they don't match the quotes surrounding the string:

Example
- print("It's alright")
- print("He is called 'Johnny'")
- print('He is called "Johnny"')

### Assign String to a Variable
Assigning a string to a variable is done with the variable name followed by an equal sign and the string:

Example
a = "Hello"
print(a)

### Multiline Strings

You can assign a multiline string to a variable by using three quotes:

Example
You can use three double quotes:

a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a)

***Or by using three single quotes:***

### Strings are Arrays
Like many other popular programming languages, strings in Python are arrays of bytes representing unicode characters.

However, Python does not have a character data type, a single character is simply a string with a length of 1.

Square brackets can be used to access elements of the string.
Example -
Get the character at position 1 (remember that the first character has the position 0):

a = "Hello, World!"
print(a[1])

### Looping Through a String
Since strings are arrays, we can loop through the characters in a string, with a for loop.

Example
Loop through the letters in the word "banana":

for x in "banana":
  print(x)

### String Length
To get the length of a string, use the len() function.

Example
The len() function returns the length of a string:

a = "Hello, World!"
print(len(a))

### Check String
To check if a certain phrase or character is present in a string, we can use the keyword in.

Example
Check if "free" is present in the following text:

txt = "The best things in life are free!"
print("free" in txt)
output - True

***Use it in an if statement:***

Example
Print only if "free" is present:

txt = "The best things in life are free!"
if "free" in txt:
  print("Yes, 'free' is present.")

### Check if NOT
To check if a certain phrase or character is NOT present in a string, we can use the keyword not in.

Example
Check if "expensive" is NOT present in the following text:

txt = "The best things in life are free!"
print("expensive" not in txt)

***Use it in an if statement:***

Example
print only if "expensive" is NOT present:

txt = "The best things in life are free!"
if "expensive" not in txt:
  print("No, 'expensive' is NOT present.")

  # Python - Slicing Strings
### Slicing
You can return a range of characters by using the slice syntax.

Specify the start index and the end index, separated by a colon, to return a part of the string.

ExampleGet your own Python Server
Get the characters from position 2 to position 5 (not included):

b = "Hello, World!"
print(b[2:5])
output - llo

### Slice From the Start
By leaving out the start index, the range will start at the first character:

Example
Get the characters from the start to position 5 (not included):

b = "Hello, World!"
print(b[:5])
output - hello

### Slice To the End
By leaving out the end index, the range will go to the end:

Example
Get the characters from position 2, and all the way to the end:

b = "Hello, World!"
print(b[2:])
output - llo, World!

### Negative Indexing
Use negative indexes to start the slice from the end of the string:
Example
Get the characters:

From: "o" in "World!" (position -5)

## Python - Modify Strings

Python has a set of built-in methods that you can use on strings.

To, but not included: "d" in "World!" (position -2):

b = "Hello, World!"
print(b[-5:-2])
output - orl

### Upper Case
ExampleGet your own Python Server
The upper() method returns the string in upper case:

a = "Hello, World!"
print(a.upper())
output - HELLO, WORLD!

### Lower Case
Example
The lower() method returns the string in lower case:

a = "Hello, World!"
print(a.lower())

## Remove Whitespace
Whitespace is the space before and/or after the actual text, and very often you want to remove this space.

Example
The **strip()** method removes any whitespace from the beginning or the end:

a = "  Hello, World! "
print(a.strip()) # returns "Hello, World!"
it removes the starting void space

## Replace String
Example
The replace() method replaces a string with another string:

a = "Hello, World!"
print(a.replace("H", "J"))
output - Jello, World!

## Split String
The split() method returns a list where the text between the specified separator becomes the list items.

Example
The split() method splits the string into substrings if it finds instances of the separator:

a = "Hello, World!"
print(a.split(",")) # returns ['Hello', ' World!']


# Python - String Concatenation

## String Concatenation
To concatenate, or combine, two strings you can use the + operator
Example - 
Merge variable a with variable b into variable c:

a = "Hello"
b = "World"
c = a + b
print(c)
output - HelloWorld

Example - 
To add a space between them, add a " ":

a = "Hello"
b = "World"
c = a + " " + b
print(c)
output - Hello World

# Python - Format - Strings


