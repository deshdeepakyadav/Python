# Python
# What is Python?
Python is a popular programming language. It was created by Guido van Rossum, and released in 1991.
It is used for:
- web development (server-side),
- software development,
- mathematics,
- system scripting.
### What can Python do?
- Python can be used on a server to create web applications.
- Python can be used alongside software to create workflows.
- Python can connect to database systems. It can also read and modify files.
- Python can be used to handle big data and perform complex mathematics.
- Python can be used for rapid prototyping, or for production-ready software development.
### Why Python?
- Python works on different platforms (Windows, Mac, Linux, Raspberry Pi, etc).
- Python has a simple syntax similar to the English language.
- Python has syntax that allows developers to write programs with fewer lines than some other programming languages.
- Python runs on an interpreter system, meaning that code can be executed as soon as it is written. This means that prototyping can be very quick.
- Python can be treated in a procedural way, an object-oriented way or a functional way.
Python Syntax compared to other programming languages
- Python was designed for readability, and has some similarities to the English language with influence from mathematics.
- Python uses new lines to complete a command, as opposed to other programming languages which often use semicolons or parentheses.
- Python relies on indentation, using whitespace, to define scope; such as the scope of loops, functions and classes. Other programming languages often use curly-brackets for this purpose.
```Example : print(“Hello Desh!”)```
Execute Python Syntax
by creating a python file on the server, using the .py file extension, and running it in the Command Line:
```C:\Users\Your Name>python myfile.py```

### Python Indentation
Indentation refers to the spaces at the beginning of a code line.
Where in other programming languages the indentation in code is for readability only, the indentation in Python is very important.
Python uses indentation to indicate a block of code.
```
if 5 > 2:
  print("Five is greater than two!")
```
Python will give you an error if you skip the indentation:
```
if 5 > 2:
print("Five is greater than two!")
```
The number of spaces is up to you as a programmer, but it has to be at least one.
```
if 5 > 2:
 print("Five is greater than two!") 
if 5 > 2:
        print("Five is greater than two!") 
```
You have to use the same number of spaces in the same block of code, otherwise Python will give you an error:
```
if 5 > 2:
 print("Five is greater than two!")
        print("Five is greater than two!")
```

## Python Variables
In Python, variables are created when you assign a value to it:
```
x = 5
y = "Hello, Desh!"
```
Python has no command for declaring a variable.
Variables do not need to be declared with any particular type, and can even change type after they have been set.
String variables can be declared either by using single or double quotes:
### Variable Names
A variable can have a short name (like x and y) or a more descriptive name (age, carname, total_volume). Rules for Python variables:
- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
- Variable names are case-sensitive (age, Age and AGE are three different variables)
```
#Legal variable names:
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"

#Illegal variable names:
2myvar = "John"
my-var = "John"
my var = "John"
```
Assign Value to Multiple Variables
Python allows you to assign values to multiple variables in one line:
```
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```
And you can assign the same value to multiple variables in one line:
```
x = y = z = "Orange"
print(x)
print(y)
print(z)
```
### Output Variables
The Python print statement is often used to output variables.
To combine both text and a variable, Python uses the + character:
```
x = "awesome"
print("Python is " + x)
```
You can also use the + character to add a variable to another variable:
```
x = 5
y = 10
print(x + y)
```
If you try to combine a string and a number, Python will give you an error:
```
x = 5
y = "John"
print(x + y)
```
### Global Variables
Variables that are created outside of a function (as in all of the examples above) are known as global variables.
Global variables can be used by everyone, both inside of functions and outside.
```
x = "awesome"
def myfunc():
  print("Python is " + x)
myfunc()
```
If you create a variable with the same name inside a function, this variable will be local, and can only be used inside the function. The global variable with the same name will remain as it was, global and with the original value.
```
x = "awesome"
def myfunc():
  x = "fantastic"
  print("Python is " + x)
myfunc()
print("Python is " + x)
```
### The global Keyword
Normally, when you create a variable inside a function, that variable is local, and can only be used inside that function.
To create a global variable inside a function, you can use the global keyword.
```
def myfunc():
  global x
  x = "fantastic"
myfunc()
print("Python is " + x)
```
Also, use the global keyword if you want to change a global variable inside a function.
```
x = "awesome"
def myfunc():
  global x
  x = "fantastic"
myfunc()
print("Python is " + x)
```
### Comments
Python has commenting capability for the purpose of in-code documentation.
Comments start with a #, and Python will render the rest of the line as a comment:
```
#This is a comment.
print("Hello, World!")
```
### Multi Line Comments
Python does not really have a syntax for multi line comments.
To add a multiline comment you could insert a # for each line:
```
#This is a comment
#written in
#more than just one line
print("Hello, World!")
```
Or, not quite as intended, you can use a multiline string.
Since Python will ignore string literals that are not assigned to a variable, you can add a multiline string (triple quotes) in your code, and place your comment inside it:
```
"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")
```
As long as the string is not assigned to a variable, Python will read the code, but then ignore it, and you have made a multiline comment.


## Built-in Data Types

In programming, data type is an important concept.
Variables can store data of different types, and different types can do different things.
Python has the following data types built-in by default, in these categories:
```
Text Type:	str
Numeric Types:	int, float, complex
Sequence Types:	list, tuple, range
Mapping Type:	dict
Set Types:	set, frozenset
Boolean Type:	bool
Binary Types:	bytes, bytearray, memoryview
```

**Setting Data Type:**
```
x = "Hello World"	#str	
x = 20	#int	
x = 20.5	#float	
x = 1j  	#complex	
x = ["apple", "banana", "cherry"]	#list	
x = ("apple", "banana", "cherry")	#tuple	
x = range(6)	#range	
x = {"name" : "John", "age" : 36}	#dict	
x = {"apple", "banana", "cherry"}	#set	
x = frozenset({"apple", "banana", "cherry"})	#frozenset	
x = True	#bool	
x = b"Hello"	 #bytes	
x = bytearray(5)	#bytearray	
x = memoryview(bytes(5))	#memoryview
```
**Getting the Data Type**
You can get the data type of any object by using the type() function:
```
x = 5
print(type(x))
```
**Setting the Specific Data Type:**
If you want to specify the data type, you can use the following constructor functions:
```
x = str("Hello World")	#str	
x = int(20)	#int	
x = float(20.5)	#float	
x = complex(1j)	#complex	
x = list(("apple", "banana", "cherry"))	#list	
x = tuple(("apple", "banana", "cherry"))	#tuple	
x = range(6)	#range	
x = dict(name="John", age=36)	#dict	
x = set(("apple", "banana", "cherry"))	#set	
x = frozenset(("apple", "banana", "cherry"))	#frozenset	
x = bool(5)	#bool	
x = bytes(5)	#bytes	
x = bytearray(5)	#bytearray	
x = memoryview(bytes(5))	#memoryview
```

## Python Numbers
There are three numeric types in Python:
- int
- float
- complex
Variables of numeric types are created when you assign a value to them:
```
x = 1    # int
y = 2.8  # float
z = 1j   # complex
```
To verify the type of any object in Python, use the type() function:
```
print(type(x))
print(type(y))
print(type(z))
```
### Int
Int, or integer, is a whole number, positive or negative, without decimals, of unlimited length.
```
x = 1
y = 35656222554887711
z = -3255522

print(type(x))
print(type(y))
print(type(z))
```
### Float
Float, or "floating point number" is a number, positive or negative, containing one or more decimals.
```
x = 1.10
y = 1.0
z = -35.59

print(type(x))
print(type(y))
print(type(z))
```
Float can also be scientific numbers with an "e" to indicate the power of 10.
```
x = 35e3
y = 12E4
z = -87.7e100

print(type(x))
print(type(y))
print(type(z))
```
### Complex
Complex numbers are written with a "j" as the imaginary part:
```
x = 3+5j
y = 5j
z = -5j

print(type(x))
print(type(y))
print(type(z))
```
### Type Conversion
You can convert from one type to another with the int(), float(), and complex() methods:
```
x = 1    # int
y = 2.8  # float
z = 1j   # complex

#convert from int to float:
a = float(x)

#convert from float to int:
b = int(y)

#convert from int to complex:
c = complex(x)

print(a)
print(b)
print(c)

print(type(a))
print(type(b))
print(type(c))
```
### Random Number
Python does not have a random() function to make a random number, but Python has a built-in module called random that can be used to make random numbers:
```
import random

print(random.randrange(1, 10))
```
## Python Casting
Specify a Variable Type
There may be times when you want to specify a type on to a variable. This can be done with casting. Python is an object-orientated language, and as such it uses classes to define data types, including its primitive types.
Casting in python is therefore done using constructor functions:
- int() - constructs an integer number from an integer literal, a float literal (by rounding down to the previous whole number), or a string literal (providing the string represents a whole number)
- float() - constructs a float number from an integer literal, a float literal or a string literal (providing the string represents a float or an integer)
- str() - constructs a string from a wide variety of data types, including strings, integer literals and float literals
```
x = int(1)   # x will be 1
y = int(2.8) # y will be 2
z = int("3") # z will be 3
x = float(1)     # x will be 1.0
y = float(2.8)   # y will be 2.8
z = float("3")   # z will be 3.0
w = float("4.2") # w will be 4.2
x = str("s1") # x will be 's1'
y = str(2)    # y will be '2'
z = str(3.0)  # z will be '3.0'
```
## String Literals
String literals in python are surrounded by either single quotation marks, or double quotation marks.
'hello' is the same as "hello".
You can display a string literal with the print() function:
```
print("Hello")
print('Hello')
```
### Assign String to a Variable
Assigning a string to a variable is done with the variable name followed by an equal sign and the string:
```
a = "Hello"
print(a)
```
### Multiline Strings
You can assign a multiline string to a variable by using three quotes:
```
a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a)
```
Or three single quotes:
```
a = '''Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua.'''
print(a)
```
