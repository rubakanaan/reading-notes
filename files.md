#  FileIO & Exceptions

<br>

## What Is a File?
*is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.*

<br>

**file systems are composed of three main parts:**

* Header: metadata about the contents of the file (file name, size, type, and so on)
* Data: contents of the file as written by the creator or editor
* End of file (EOF): special character that indicates the end of the file

<br>

## Opening and Closing a File in Python

* **open()** has a single required argument that is the path to the file. **open()** has a single return, the file object:

* for example : **file = open('dog_breeds.txt')**

* There are three different categories of file objects:

* Text files

* Buffered binary files

* Raw binary files

<br>
<br>
<br>


# Python Exceptions.
<br>

***A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception***

<br>

## Exceptions versus Syntax Errors

* **Syntax errors** occur when the parser detects an incorrect statement.
* **exception error:** This type of error occurs whenever syntactically correct Python code results in an error.

<br>

## Raising an Exception
* We can use **raise** to throw an exception if a condition occurs. The statement can be complemented with a custom exception.

<br>

## The try and except Block: Handling Exceptions
* The **try** and **except** block in Python is used to catch and handle exceptions. Python executes code following the **try** statement as a “normal” part of the program. The code that follows the **except** statement is the program’s response to any exceptions in the preceding **try** clause.

* A **try** clause is executed up until the point where the first exception is encountered.

* Inside the **except** clause, or the exception handler, you determine how the program responds to the exception.

* You can anticipate multiple exceptions and differentiate how the program should respond to them.

<br>

## The else Clause
* In Python, using the **else** statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.

<br>

## Cleaning Up After Using finally
Imagine that you always had to implement some sort of action to clean up after executing your code. Python enables you to do so using the **finally** clause.