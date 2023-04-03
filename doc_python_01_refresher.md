---
layout: default
title: __Bonus - Python Refresher
# parent: Python Programming
nav_order: 99

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




## Why Python?

As stated in the [official page of python](https://www.python.org/doc/essays/blurb/):\
"Python is one of the world’s most used and most popular programming languages. It’s powerful, versatile, and easy to 
learn. Python is widely used in various applications, some notable ones:
- Web development
- Data Science
- Data analysis
- Machine learning
- Artificial Intelligence (AI)
- Scripting and tooling"

For this course, we expect you to have basic knowledge of the Python programming language. If you need a refresher, 
we have you covered! Just keep reading. 

## Python pros and cons
Python is a distinctive programming language that has both advantages and disadvantages, making it a good choice 
for certain situations and not as good for others. This section will outline the positive attributes of Python. Below, you 
will find a summary of advantages and disadvantages of Python as a programming language. What follows was inspired by 
[linode.com](https://www.linode.com/docs/guides/pros-and-cons-of-python/) where you can read more. 

### Advantages

1. *Ease of use.* One of Python's most significant benefits is its ease of use. Its syntax is simple, concise, 
and straightforward, making it highly readable and easy to debug. Python's control structures are intuitive and 
easy to use. Moreover, Python is dynamically typed, which eliminates the need to declare the type of each 
variable, resulting in more efficient and productive programming.

2. *Learning curve.* Python also has a gentle learning curve, making it a good option for 
individuals learning to program. Programmers who switch to Python from other languages such as C or Java can quickly reach peak efficiency, and the Python package includes a useful Integrated Development and Learning Environment (IDLE).

3. *Versatility.* Python is a versatile, general-purpose language that supports both procedural and 
object-oriented programming. Its built-in and third-party packages make it suitable for a wide range of tasks. 
Python is dominant in the areas of data science and machine learning and is widely used for back-end web development 
and the Internet of Things (IoT). It is even possible to embed Python code into projects written in other languages, 
such as C++, and vice versa.

4. *Rapid development and efficiency*. Python is efficient for rapid development because it is easy to use and 
does not require compilation, which saves time. Python programs are often much shorter than equivalent programs 
in other languages, making it an excellent choice for constructing prototypes quickly in a rapid software 
development environment. 

5. *Portability*. Python is also true portable, meaning it can be written once and run anywhere. 
Python does not need to be compiled in advance, so users run a true Python program rather than a Python executable. 
The program is not compiled until it is run using the platform-specific PVM. This means that any Python program can 
potentially run on any system that supports Python.

6. *No compile process*. Python's interpreted language does not require a separate compiler or time-consuming 
compilation step, so programs can be run as soon as they are written. This makes Python programs easy to write, 
debug, and change incrementally. Additionally, Python's automatic memory allocation eliminates the need for developers 
to assign free space in memory. A garbage collector recycles memory from discarded objects, eliminating worries about 
scribblers, memory leaks, invalid pointer references, or object size.

7. *Automatic memory allocation*. Python has a large number of built-in compound objects, including lists, sets, 
and record-like dictionaries, each providing a collection of methods for easy processing. Moreover, Python has an 
extensive library containing tens of thousands of functions that can be used for network communications, 
web integration, data processing, and hardware interactions. This library reduces the time spent writing programs 
as many necessary routines have already been written.

8. *Extensive built-in objects and libraries*. Python has many free external libraries that developers 
can access in addition to its extensive built-in library. These third-party libraries are easy to import and install 
using Python's pip package manager, which can be downloaded from the Python Package Index (PyPI) repository. 
PyPI also allows developers to publish their packages.

9. *Third-party library availability*. All Python releases are available for free under an open-source license. 
Python can even be modified and re-distributed at no cost, making it a low-cost option for developers. 

11. *User base*. Python has a large, active, and passionate community of users, making it easy to find learning 
materials and other resources, ask questions, search for jobs, hire additional developers, and meet other Python 
programmers.

### Disadvantages

Despite its many advantages, Python also has a few notable disadvantages. These will be discussed in the next section.

1. *Slow Performance.* Compared to more efficient programming languages like C and Java, Python is significantly slower 
due to its interpretation and dynamic typing. This makes it unsuitable for situations where speed is critical.

2. *High Memory Usage.* Python is not optimized to reduce memory and can consume up to ten times more RAM than 
programs written in more frugal languages. The garbage collector in Python cannot immediately gather all discarded resources, which also reduces the amount of available memory. This makes it unsuitable for memory-constrained environments.

3. *Difficulties in Avoiding Runtime Errors.* Python is not compiled until runtime and is dynamically typed, which 
means that many errors that would be caught by the compiler in other languages do not appear until the program runs.

4. *Limited Traction in Mobile and Desktop Applications.* Python has not made significant progress in the mobile 
space due to its slower speed and high memory usage. Although there are some Python development tools for mobile apps, they are more limited than frameworks for other languages. Python is also not very popular for front-end applications in client desktops.

5. *Not Optimized for Database Access.* Python lacks a powerful, high-quality, easy-to-use interface for 
working with databases, which makes it more challenging to work with databases than some other applications. 
It can still be used if the database reads and writes are relatively straightforward, but it is not the best choice 
for applications that have complex interactions with a large corporate database.

6. *No Multithreading Support.* Python does not support multithreading due to its architecture. Instead, it relies on 
multiprocessing, where each "thread" runs in a separate Python process. This can result in uneven performance and 
relies on the operating system to schedule and balance the processes.

7. *Prone to Overuse or Misuse.* Python's simplicity can sometimes lead to overuse or misuse, especially for tasks 
where it is not the best option. While it is great for rapid development and prototypes, organizations should not 
overlook proper software development principles.

## Getting started
### Installing Python and quickstarting
There are many ways to install Python. We recommend using [Miniconda](https://docs.conda.io/en/latest/miniconda.html),<sup>*</sup> 
which will install Python alongside some useful packages. Make sure to use Python 3 (e.g., v.3.7 or superior). 

To check if Python was successfully  installed, you can use the following commands:\
On a Windows computer (command line):\
```C:\Users\Your Name>python --version```

On a Mac or Linux computer (terminal):\
```$ python --version```

Congrats! Now you have installed Python! You can find examples and exercises on how to get started with Python on the
[W3schools](https://www.w3schools.com/python/python_getstarted.asp) website, in the 
[Python Getting Started](https://www.w3schools.com/python/python_getstarted.asp) page.

<sup>*</sup><u>Spoiler Alert!</u> Miniconda will be useful to install additional packages you might need, see the [Tools](doc_python_02_tools.md) page.

### Nice-to-haves

Other few ingredients will make your life easier and more fun while coding. They are:
1. A Python IDE, to write better code, faster. Have a look at the [tools](doc_python_02_tools.md) page, in the IDE section.
2. A package manager , such as Conda. See [tools](doc_python_02_tools.md) page.
3. A computer! 💻

## Python syntax

### Basic syntax
<details close markdown="block">
  <summary>
    Expand
  </summary>

The examples below are taken from the [official Python documentation](https://docs.python.org/3/tutorial/introduction.html#first-steps-towards-programming), 
where you will find even more!

**Numbers and operations**
The interpreter acts as a simple calculator: you can type an expression at it, and it will write the value. 
Expression syntax is straightforward: the operators `+`, `-`, `*` and `/` are used to perform calculation, 
and the parentheses (`()`) are for grouping. For example:

```python
>> 2 + 2
4
>> 50 - 5*6
20
>> (50 - 5*6) / 4
5.0
>> 8 / 5  # division always returns a floating point number
1.6
```
Division (`/`) always returns a float. To do floor division and get an integer result you can use the `//` operator; 
to calculate the remainder you can use `%`:

```python
>> 17 / 3  # classic division returns a float
5.666666666666667
>> 17 // 3  # floor division discards the fractional part
5
>> 17 % 3  # the % operator returns the remainder of the division
2
>> 5 * 3 + 2  # floored quotient * divisor + remainder
17
```

With Python, the `**` operator can be used to calculate powers:
```python
>> 5 ** 2  # 5 squared
25
>> 2 ** 7  # 2 to the power of 7
128
```

The equal sign (`=`) is used to assign a value to a variable.
```python
>> width = 20
>> height = 5 * 9
>> width * height
900
```

<u>Warning!</u> The operator `=` should not be confused with `==`, which is used to compare objects based on their values:
```python
>> width = 20  # assigns the value the variable
>> width == 25 # compares it with 25
False
```

**Strings**

Besides numbers, Python can also manipulate strings, which can be expressed either with single (`'`) or double (`"`) quotes
with the same result. `\` can be used to escape quotes:
```python
>> 'mountain trail'  # single quotes
'mountain trail'
>> 'doesn\'t'        # use \' to escape the single quote
"doesn't"
>> "doesn't"         # or use double quotes instead
"doesn't"
>> '"No," they said.'
'"No," they said.'
>> "\"No,\" they said."
'"No," they said.'
>> '"Isn\'t," they said.'
'"Isn\'t," they said.'
```
Strings can be concatenated  with the `+` operator, and repeated with `*`:
```python
>> 'sci' + 'ence'         # concatenation
'science'
>> 2*'da'                 # repetition
'dada'
>> 2 * 'per' + 'petual'   # repetition and concatenation
'perpetual'
```
**Lists**

Lists are a versatile way to group values together. 
With lists, comma-separated values (items) are specified between square brackets. 
Lists might contain items of different types, but usually the items all have the same type.
```python
>> values = [1, 2, 5]
values
[1, 2, 5]
```
Lists can be indexed and sliced:
```python
>> values = [1, 2, 5]
>> squares[0]          # indexing returns the item
1
>> values[-2:]         # slicing returns a new list
[2,5]
```
If you are confused about the values returned in the previous example, you're not alone. Keep reading until the indexing
section below.

Lists also support operations like concatenation:
```python
>> values + [27, 28]
[1, 2, 5, 27, 28]
```

You can also change the content of a list:
```python
>> values
[1, 2, 5]
>> values[0] = 40
>> values
[40, 2, 5]
```
You can add new items at the end of the list, by using `append()`, and count the items it contains with `len()`: 
```python
>> values              # displays the list
[40, 2, 5]
>> len(values)         # counts the number of items
3
>> values.append(100)  # appends a new item
>> values              # displays the list again
[40, 2, 5, 100]
>> len(values)         # counts the number of items again
4
```

**Python indexing and slicing**
If you come from other programming languages such as [MATLAB](), [Julia](), or [R],(), you might be surprised to discover
that Python starts counting from 0. 
```python
>> a = ['cat', 'dog', 'mouse', 'monkey']
>> a[0]             # first element of the list
'cat'
>> a[1]             # second element of the list
'dog'
>> a[len(a)-1]      # ultimate element (lenght - 1) of the list
'monkey'
>> a[:]             # entire list
['cat', 'dog', 'mouse', 'monkey']
```
You can also use negative numbers for indexing, which starts to count from the end of the sequence:

```python
>>> a[-1]
'monkey'
>>> a[-2]
'mouse'
>>> a[-4]
'cat'
```


<u>NB!</u> If you need more examples, you can have a look at the [Python Cheatsheet](https://www.pythoncheatsheet.org/), among others.

</details>

### Indentation
<details close markdown="block">
  <summary>
    Expand
  </summary>

Indentation refers to the spaces at the beginning of a code line. Whereas other programming languages use indentation 
for readability, in Python, indentation is a key element of the syntax. In fact, Python uses indentation to indicate a block of code.

```python
# Correct usage of indentation
a = 10
if 10 > 3:
  print("a is greater than three!")
  if a > 9:
      print("a is also greater than 9")

      
# This would give a syntax error  
if 10 > 3:
print("Ten is greater than three!")
if a > 9:
print("a is also greater than 9")
```

The number of spaces is up to you as a programmer, but it has to be at least one! Also, check out [Writing good Python code > Python PEP8 Style Guide](#doc_python_style)
on suggestions regarding the 'stylistic' usage of spaces. 
</details>

### Variables, types, and casting
<details close markdown="block">
  <summary>
    Expand
  </summary>

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
Casting in Python is rather easy, and can be done with the following functions:
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

<details close markdown="block">
  <summary>
    Click here to expand the selected keywords
  </summary>

| Keyword    |                   Function                   |                                                                             Description | Examples<sup>*</sup>                           |
|------------|:--------------------------------------------:|----------------------------------------------------------------------------------------:|------------------------------------------------|
| `and`      |               Logical operator               |                                          Returns `True` if two statements are both true | `x < 5 and  x < 10`                            |
| `as`       |                Import keyword                |                        When importing a module with `import`, specifies the name to use | `import pandas as pd`                          |
| `assert`   |          Diagnostics and execution           |                             If a condition returns `False`, an AssertionError is raised | `assert x == "goodbye", "x should be 'hello'"` |
| `break`    |              Function for loops              |                                                             Terminates the current loop | See [loops](#loops).                           |
| `class`    |                Class keyword                 |                                                                  Used to create classes | -                                              |
| `continue` |              Function for loops              | Ends the current iteration in a `for`(or `while` ), and continues to the next iteration | -                                              |
| `def`      |               Function keyword               |                                                                       Defines functions | See [functions](#functions).                   |
| `elif`     |          Keyword for if statements           |        Specifies the condition for if statements, when more than one alternative exists | See [logical conditions](#logical_conditions). |
| `else`     |          Keyword for if statements           |                            Specifies the condition as an alternative to an if statement | See [logical conditions](#logical_conditions). |
| `except`   |             Try-except statement             |                  Used to continue the execution when an error is encountered, see `try` | -                                              |
| `False`    |             Comparison operator              |               Boolean value resulting from a comparison operation. (Opposite of `True`) | -                                              |
| `for`      |              Function for loops              |                                            Specifies the values to iterate on in a loop | See [loops](#loops).                           |
| `from`     |                Import keyword                |                                     Used to import only a specified section of a module | `from pandas import DataFrame`                 |
| `if`       |          Keyword for if statements           |                                            First condition specified in an if statement | See [logical conditions](#logical_conditions). |
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
| `while`    |              Function for loops              |                             Executes a set of statements as long as a condition is true | See [loops](#loops)                            |

<sup><sup>*</sup> Only simple, one-line examples are provided. 😊 Bear with us!</sup>

</details>
</details>

## Fundamentals of Python programming

### Logical conditions

<details close markdown="block">
  <summary>
    Click here to expand
  </summary>

**Mathematical conditions**
Python supports simple logical conditions, such as:
* Equals: `a == b`
* Does not Equal: `a != b`
* Less than: `a < b`
* Less than or equal to: `a <= b`
* Greater than: `a > b`
* Greater than or equal to: `a >= b`

**If statements** 

The `if` statements are used to specify specific behaviours when one (or more) condition(s) are satisfied.

You can specify a single condition, for instance:
```python
a = 40
b = 100
if b > a:
  print("b is larger than a")
```

If you want to specify more than one condition, you can combine `if` and `else`:
```python
a = 40
b = 100
if b > a:
  print("b is larger than a")
else:
  print("b is not larger than a")
```

To specify more than two conditions, you can use `elif` (else-if), too:
```python
a = 40
b = 100
if b > a:
  print("b is larger than a")
elif b < a:
  print("b is smaller than a")
else:
  print("b is equal to a")
```

</details>

### Loops
<details close markdown="block">
  <summary>
    Click here to expand
  </summary>

A loop is a sequence of instructions that is continually repeated until a certain condition is reached. In Python,
this can be achieved using `for` or `while` statements.

**'For' loops** 

A `for` loop is used for iterating over a sequence (that is either a list, a tuple, a dictionary, a set, or a string).

```python
# Print each fruit in a fruit list:
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)

# Loop through the letters in the word "banana":
for x in "banana":
  print(x)
```

Loops can be exited using the `break` statement:
```python
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break
```
**'While' loops** 

The `while` executes a set of statements as long as the specified condition is true.

```python
# prints the value of i starting from 1 and terminating at 9
i = 1
while i < 10:
  print(i)
  i += 1 
```

Also in this case, you can use the `break` statement:
```python
# prints the value of i starting from 1 and terminates the loop when i is 4
i = 1
while i < 10:
  print(i)
  if i == 4:
    break
  i += 1
```
</details>

### Functions
<details close markdown="block">
  <summary>
    Click here to expand
  </summary>
A function is a block of code that runs only when it is called. You can pass data (known as parameters), into a function.
In python, functions are defined using the `def` keyword, as follows:

```python
def hello():
  print("Hello world!")
```
This function will be called as `hello()`, and will print the specified string. 
```
>>> hello()
Hello world!
```
**Function arguments**

Information can be passed into functions as arguments, for instance:
```python
def hello(name):
  print("Hello " + name + "!")
```
Which would result in the following:
```
>>> hello("Michael")
Hello Michael!

>>> hello("Meilina")
Hello Meilina!
```
More than one parameter can be allowed, for instance:
```python
def hello(first_name, last_name):
  print("Hello " + first_name + " " + last_name + "!")
```
results in the following:
```
>>hello("LeBron","James")
Hello LeBron James!
```

**Arbitrary arguments** (`*args`)

If you do not know how many arguments that will be passed into your function, add a `*` before the parameter name in 
the function definition. In this way the arguments will be passed as a *tuple*, and you can access the items accordingly:
```python
def smallest(*ages):
  print(str(min(ages))) # computes the minimum and converts to a string for printing
```
results in the following:
```
>>smallest(1,2,3)
1
>>smallest(-100,1,2,3,100)
-100
```

**Arbitrary arguments** (`**kwargs`)

`**kwargs` (key word arguments) works like `*args`, but instead of accepting positional arguments it accepts keyword (or named) arguments.

```python
def person_details(**kwargs):
    print(kwargs, type(kwargs))
```
results in the following:
```
>>person_details(name="LeBron", surname="James", height=2.06)
{'surname': 'James', 'name': 'LeBron', 'height': 2.06}

>>person_details(name="Peppa", surname="Pig", DoB="May 30")
{'DoB': 'May 30', 'surname': 'Pig', 'name': 'Peppa'}
```
</details>

## References
This page was inspired by many awesome resources available online, and in particular by:  \
* [W3schools](https://www.w3schools.com/python/python_variables_multiple.asp)
* [A Byte of Python](https://python.swaroopch.com/)


## Additional resources
* [Book] [A Byte of Python](https://python.swaroopch.com/):  a free book on programming using the Python language. It serves as a tutorial or guide to the Python language for a beginner audience.
* [Online tutorial] [Learn Python Programming](https://pythonbasics.org/): a website containing materials and exercises for the Python 3 programming language.
* [Online quizzes] [HackerRank](https://www.hackerrank.com/dashboard), a great platform to test you coding knowledge and solve challenging problems!


<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>
