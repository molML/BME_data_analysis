---
layout: default
title: Writing good Python code
parent: Python Programming
nav_order: 99
---

# Writing Good Python code
{: .no_toc }


<img src="https://www.explainxkcd.com/wiki/images/0/06/bad_code.png" width=500>

<sup>Image credits [xkcd](https://www.explainxkcd.com/wiki/index.php/1926:_Bad_Code)</sup>

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

---

## Writing good Python code

1. *Write clear and concise code*:
Python is a highly readable language, so aim to make your code as clear and concise as possible. Use meaningful variable names, avoid redundancy, and break down complex tasks into smaller functions.

2. *Follow PEP8 guidelines*: As mentioned earlier, the PEP8 guidelines outline best practices for writing Python code. Following these guidelines can help make your code more consistent and easier to read.

3. *Use built-in functions and libraries*:
Python has a rich standard library with many built-in functions and modules that can simplify your code and reduce the amount of code you need to write. Don't reinvent the wheel if you don't have to.

4. *Be mindful of performance*:
Python is a relatively slow language compared to some other languages, so it's important to be mindful of performance when writing code. For example, use list comprehensions instead of for loops whenever possible and avoid unnecessary object creation.

5. *Write unit tests*:
Unit tests are a great way to ensure that your code works as intended and to catch bugs before they become a problem. Aim to write tests for every function you write and test edge cases to ensure your code is robust.

6. *Document your code*:
Clear documentation can help others understand your code and make it easier to maintain. Use comments to explain what your code is doing, write docstrings for functions and classes, and consider using a tool like Sphinx to generate documentation automatically.

7. *Use version control*:
Version control is an essential tool for managing code and collaborating with others. Use a version control system like Git to track changes to your code, collaborate with others, and easily roll back changes if needed.

These are just a few tips for writing good Python code. By following these best practices and continuously learning and improving your coding skills, you can write code that is efficient, maintainable, and easy to read.

## Python PEP8 Style

Python PEP8 style is a set of guidelines for writing Python code that promotes consistency and readability. 
PEP stands for *"Python Enhancement Proposal"*, which is proposes a standard style for Python code.

The PEP8 style guide covers various aspects of Python code, including naming conventions, whitespace, comments, and more. 
Here are some of the key guidelines:

1. Naming Conventions:
- Variables, functions, and modules should be named in lowercase, with underscores separating words, for example, my_variable.
- Class names should be in CamelCase, where the first letter of each word is capitalized, for example, MyClass.
2. Indentation and Whitespace:
- Indentation should be 4 spaces. Avoid using tabs.
- Avoid trailing whitespaces.
3. Comments:
- Use comments sparingly and only where necessary.
- Use complete sentences and punctuation in comments.
4. Line Length:
- Lines should be no longer than 79 characters.
- When a line is too long, it can be continued on the next line using parentheses.
5. Function and Class Structure:
- Function and class definitions should be separated by two blank lines.
- Class methods should have their first parameter named "self".
- Use empty lines to separate logical sections of code within functions.

These are just a few of the guidelines outlined in the PEP8 style guide. 
By adhering to these guidelines, your code will be more readable and consistent, making it easier for other developers 
to understand and work with your code. 

To further aid in adhering to the PEP8 style, there are a number of tools and plugins available that can automatically 
check and correct your code style. Some popular ones include Flake8, Black, and Pylint.

PEP8 is a set of guidelines for writing Python code that promote consistency and readability. 
By following these guidelines, you can make your code more readable and easier for others to understand and work with.
You can know more on the official [PEP8](https://peps.python.org/pep-0008/) page.


## Make your code more Pythonic

Can you provide suggestion on how to make the code more Pythonic?

Use List Comprehensions:
List comprehensions allow you to create new lists based on existing ones using a concise syntax. For example, instead of using a for loop to create a new list of squares, you can use a list comprehension like this:
css
Copy code
squares = [x**2 for x in range(10)]
Use Generators:
Generators are a way to create iterators in a concise way. They allow you to generate a sequence of values on-the-fly instead of creating the entire sequence upfront. This can be useful when dealing with large datasets or when memory is a concern. For example:
csharp
Copy code
even_numbers = (x for x in range(10) if x % 2 == 0)
Use Context Managers:
Context managers are a way to manage resources like files or database connections in a safe and efficient way. They ensure that resources are properly initialized and cleaned up after use. For example:
csharp
Copy code
with open('myfile.txt', 'r') as f:
    data = f.read()
Use Default Arguments:
Default arguments allow you to provide a default value for a function parameter. This can simplify your code by eliminating the need for conditional statements to handle missing arguments. For example:
python
Copy code
def greet(name='World'):
    print(f'Hello, {name}!')

greet() # outputs 'Hello, World!'
greet('Alice') # outputs 'Hello, Alice!'
Use Decorators:
Decorators allow you to modify the behavior of a function or class without changing its source code. This can be useful for adding functionality like logging, caching, or authentication. For example:
python
Copy code
def memoize(func):
    cache = {}

    def wrapper(*args):
        if args not in cache:
            cache[args] = func(*args)
        return cache[args]

    return wrapper

@memoize
def fibonacci(n):
    if n in (0, 1):
        return n
    return fibonacci(n-1) + fibonacci(n-2)
These are just a few examples of how you can make your code more Pythonic. In general, try to write code that is concise, readable, and takes advantage of the language's built-in features and libraries.
https://towardsdatascience.com/5-things-that-will-instantly-make-your-python-code-more-pythonic-198c6d371c80
https://docs.python-guide.org/writing/style/

<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>
