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

Python supports different types of variables:
* whole integers (e.g., 3)
* floating point numbers (e.g., 3.1415926)
* booleans (true or false)
* strings (text) (e.g., "Python")

You do not need to specify the datatype of a variable, you can simply assign any value to a variable. 
Try with the exercise below:

```python
x = 3              # a whole number                   
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

A variable name <u>must</u> begin with a letter (upper or lower case) or an underscore. Variables cannot start with a number 
and are case-sensitive.





## Fundamentals of python programming




## References and acknowledgements
This page was inspired by many awesome resources available online, and in particular by:  \
*[W3schools](https://www.w3schools.com/python/python_variables_multiple.asp)
*[A Byte of Python](https://python.swaroopch.com/)

## Additional resources
* [Book] [A Byte of Python](https://python.swaroopch.com/):  a free book on programming using the Python language. It serves as a tutorial or guide to the Python language for a beginner audience. 
* [Online tutorial] [Learn Python Programming](https://pythonbasics.org/): a website containing materials and exercises for the Python 3 programming language.

<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>
