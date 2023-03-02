---
layout: default
title: Python Refresher
parent: Python Programming
nav_order: 1
---

# Python Refresher
{: .no_toc }

For the scopes of this course, we assume you have basic knowledge of the python programming language. If you don't have basics of Python, 
have a look at the [additional resources](#additional-resources) section. If you just need a 
refresher, no problem, we have you covered! Just keep reading... 

<p align="center">
<img src="https://images.pexels.com/photos/4378128/pexels-photo-4378128.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" width=300>
</p>

## Contents
{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

---



## Getting started
### Installing Python and quickstarting
There are many ways to install Python. We recommend using [Miniconda](https://docs.conda.io/en/latest/miniconda.html),<sup>*</sup> 
which will install Python alongside some useful packages. Make sure to use Python 3 (e.g., v.3.7 or superior). 

To check if Python was successfully  installed, you can use the following commands:\
On a Windows computer (command line):\
```C:\Users\Your Name>python --version```

On a Mac or Linux computer (terminal):\
```python --version```

Congrats! Now you have installed Python! You can find examples and exercises on how to get started with Python on the
[W3schools](https://www.w3schools.com/python/python_getstarted.asp) website, in the 
[Python Getting Started](https://www.w3schools.com/python/python_getstarted.asp) page.

<sup>*</sup><u>Spoiler Alert!</u> Miniconda will be useful to install additional packages you might need, see the [Tools](doc_python_02_tools) page.

### Nice-to-haves

Other few ingredients will make your life easier and more fun while coding. They are:
1. A Python IDE, to write better code, faster. Have a look at the [IDE Section](doc_python_02_tools).
2. A package manager, such as Conda (see #TODO).
3. A computer!

## Python syntax

### Basic syntax

### Indentation

### Variables, types, and casting
\
**Variable types**

Python supports different types of variables:
* whole integers (e.g., 3)
* floating point numbers (e.g., 3.1415926)
* booleans (true or false)
* strings (text) (e.g., "Python")

You do not need to specify the datatype of a variable, you can simply assign any value to a variable. 
Try with the exercise below:

```python
x = 3              # an integer                   
f = 3.1415926      # a floating point number              
name = "Python"    # a string

print(x)
print(f)
print(name)

combination = name + " " + name
print(combination)

sum = f + f
print(sum)
```

**Variable casting**

There may be cases in which you want to specify a type on to a variable. 
Casting in python is rather easy, and can be done with the following functions:
* `int()` constructs an integer number from an integer, a float (by removing all decimals), or a string (providing the string represents a whole number).
* `float()` constructs a float number from an integer, a float or a string (providing the string represents a float or an integer).
* `str()` - constructs a string from a wide variety of data types, including strings, integer literals and float literals.

See the example below (taken from [W3schools](hhttps://www.w3schools.com/python/python_casting.asp)):
```python
# Integers
x = int(1)       # x will be 1
y = int(2.8)     # y will be 2
z = int("3")     # z will be 3

# Float numbers
x = float(1)     # x will be 1.0
y = float(2.8)   # y will be 2.8
z = float("3")   # z will be 3.0
w = float("4.2") # w will be 4.2

# Strings
x = str("s1")    # x will be 's1'
y = str(2)       # y will be '2'
z = str(3.0)     # z will be '3.0'
```


**Naming variables**

A variable name <u>must</u> begin with a letter (upper or lower case) or an underscore. Variables cannot start with a number 
and are case-sensitive. Several conventions for names exist, such as capitalized words (also known as camel-casing), lower-letters,
capitalization. 

```python
MyBelovedVariable = 3    # camel case                   
mybelovedvariable = 4    # lower letter
MYBELOVEDVARIABLE = 5    # capitalized
```

On Style

**Python operators**

Python has 35 reserved words that cannot be used as variable names. Here are some of the ones that will be useful for you. 
A full list can be found [here](https://en.wikipedia.org/wiki/Python_syntax_and_semantics). 

| Keyword    |                   Function                   |                                                                             Description | Examples<sub>*</sub>                           |
|------------|:--------------------------------------------:|----------------------------------------------------------------------------------------:|------------------------------------------------|
| `and`      |               Logical operator               |                                          Returns `True` if two statements are both true | `x < 5 and  x < 10`                            |
| `as`       |                Import keyword                |                        When importing a module with `import`, specifies the name to use | `import pandas as pd`                          |
| `assert`   |          Diagnostics and execution           |                             If a condition returns `False`, an AssertionError is raised | `assert x == "goodbye", "x should be 'hello'"` |
| `break`    |              Function for loops              |                                                             Terminates the current loop | -                                              |
| `class`    |                Class keyword                 |                                                                  Used to create classes | -                                              |
| `continue` |              Function for loops              | Ends the current iteration in a `for`(or `while` ), and continues to the next iteration | -                                              |
| `def`      |               Function keyword               |                                                                       Defines functions | -                                              |
| `elif`     |          Keyword for if statements           |        Specifies the condition for if statements, when more than one alternative exists | -                                              |
| `else`     |          Keyword for if statements           |                            Specifies the condition as an alternative to an if statement | -                                              |
| `except`   |             Try-except statement             |                  Used to continue the execution when an error is encountered, see `try` | -                                              |
| `False`    |             Comparison operator              |               Boolean value resulting from a comparison operation. (Opposite of `True`) | -                                              |
| `for`      |              Function for loops              |                                            Specifies the values to iterate on in a loop | -                                              |
| `from`     |                Import keyword                |                                     Used to import only a specified section of a module | `from pandas import DataFrame`                 |
| `if`       |          Keyword for if statements           |                                            First condition specified in an if statement | -                                              |
| `import`   |                Import keyword                |                                                Imports a module, by making it available | `import pandas`                                |
| `in`       |             Membership operator              |          Returns `True` if a sequence with the specified value is present in the object | `x in y` or  `x not in y`                      |
| `is`       |              Identity operator               |                                                          Comparison between two objects | `x is y`                                       |
| `is not`   |              Identity operator               |                                                          Comparison between two objects | `x is not y`                                   |
| `None`     |                 None keyword                 |                                                                     Define a null value | `x = None`                                     |
| `or`       |               Logical operator               |                                        Returns `True` if one of two statements is  true | `x < 5 or  x > 10`                             |
| `raise`    |          Diagnostics and execution           |      Raises an error and stops the program if a condition is satisfied (e.g., via `if`) | -                                              |
| `return`   |               Function keyword               |                                      Sends the results of a function back to the caller | -                                              |
| `True`     |             Comparison operator              |              Boolean value resulting from a comparison operation. (Opposite of `False`) | -                                              |
| `try`      |             Try-except statement             |                             Used to continue the execution when an error is encountered | -                                              |
| `while`    |              Function for loops              |                             Executes a set of statements as long as a condition is true | -                                              |



<sub>*</sub> Only simple, one-line examples are provided. 😊 Bear with us!


## Fundamentals of python programming




## References and acknowledgements
This page was inspired by many awesome resources available online, and in particular by:  \
*[W3schools](https://www.w3schools.com/python/python_variables_multiple.asp)
*[A Byte of Python](https://python.swaroopch.com/)

## Additional resources
* [Book] [A Byte of Python](https://python.swaroopch.com/):  a free book on programming using the Python language. It serves as a tutorial or guide to the Python language for a beginner audience. 
* [Online tutorial] [Learn Python Programming](https://pythonbasics.org/): a website containing materials and exercises for the Python 3 programming language.

<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>
