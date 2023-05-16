---
layout: default
title: Object-oriented Programming
nav_order: 3
---

# Object-oriented Programming with Python
{: .no_toc }

<img src="https://realpython.com/cdn-cgi/image/width=960,format=auto/https://files.realpython.com/media/Object-Oriented-Programming-OOP-in-Python-3_Watermarked.0d29780806d5.jpg" width=800>

<sup>Image credits [Real Python](https://realpython.com/python3-object-oriented-programming/)</sup>


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
Below, you will find a short summary of OOP, what it allows you to achieve, along with some examples in Python code.

## Why object-oriented programming?
Object-oriented programming (OOP) is a programming paradigm that focuses on organizing code into objects, each of which encapsulates data and behavior. This allows for more modular and flexible code, as well as easier reuse of code across different parts of a program. OOP is one of the most popular programming paradigms in use today, and is widely used in a variety of domains, including software engineering, game development, and data science.
One of the key benefits of OOP is that it provides a way to organize code 
into reusable, modular units that are easy to understand and modify.

Several keywords are useful to understand OOP:
- Classes, which define the blueprint for creating objects. 
- Object, an instance of a class, which contains its own set of properties and methods.
- Properties (or attributes) are the data members of a class.
- Methods are the functions that operate on the properties of a class.

When we create an object in OOP, we are instantiating it from a class. Instantiation is the process of creating an object 
from a class. This allows us to create multiple instances of the same class, each with its own set of properties and methods.

One of the advantages of OOP is that it allows us to create objects with properties that can be easily modified without
affecting other parts of the program. This is because properties are encapsulated within the object and can only be accessed through its methods. This makes it easier to maintain and modify code, as we can make changes to the properties of a specific object without affecting other objects in the program.

Methods in OOP are functions that operate on the data members of a class. They can be used to manipulate data, 
perform calculations, or interact with other objects in the program. Methods can be defined at the class level, which means that all instances of that class will have access to the same set of methods.

Overall, OOP is an important concept in programming because it allows us to create reusable, modular units of code. By encapsulating 
data and behavior within objects, we can create code that is easier to understand and modify. Additionally, instantiation 
allows us to create multiple instances of the same class, each with its own set of properties and methods. This makes 
it easier to maintain and modify code, as we can make changes to specific objects without affecting the rest of the program.

## The four principles of OOP
The four principles of object-oriented programming (OOP) are:

1. Encapsulation. This principle refers to the concept of encapsulating data and behavior within an object. This means that the data and methods of an object are kept together, making it easier to manage and modify them. Encapsulation allows us to hide the implementation details of an object, and only expose the interface that other objects can interact with.
2. Abstraction. This principle refers to the ability to define abstract classes or interfaces that provide a high-level description of objects, without getting into the details of their implementation. Abstraction allows us to create classes that are more flexible and adaptable to changes, as we can modify the implementation details without affecting other parts of the program.
3. Inheritance. This principle refers to the ability to create new classes based on existing classes. Inheritance allows us to create classes that inherit the properties and methods of their parent classes, making it easier to reuse code and build on existing functionality. Inheritance is also useful for creating hierarchies of classes, where more specialized classes inherit from more general ones.
4. Polymorphism. This principle refers to the ability to create classes that can take on multiple forms. Polymorphism allows us to define methods that can be used with multiple types of objects, making the code more flexible and adaptable. Polymorphism is often used in conjunction with inheritance, where a method in a parent class can be overridden by a method in a child class, providing different behavior for different types of objects.

## OOP in Python
Below, are some examples on how Python can be used for OOP. These examples are not meant to be exhaustive, but just to
provide you with a flavour of how to use OOP with Python. To know more, have a look at the Additional Resources below.

### Main things to know about OOP in Python
Below are some things to keep in mind when starting with Python and OOP, along with code examples. You will find a comprehensive
tutorial with step-by-step exercises at [Real Python](https://realpython.com/python3-object-oriented-programming/).

**1. Understanding classes and objects:**

In Python, everything is an object. A class is a blueprint for creating objects, while an object is an instance of a class. 
To create a class in Python, we use the `class` keyword, followed by the class name and a colon. 
We define the attributes of the class in the `__init__` method, and we define the methods of the class as functions within the class. 
Here is an example:

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def say_hello(self):
        print("Hello, my name is " + self.name + " and I am " + str(self.age) + " years old.")

p1 = Person("Alice", 25)
p1.say_hello()  # prints "Hello, my name is Alice and I am 25 years old."
```

**2. Inheritance:** 

Inheritance is a way to create a new class from an existing class, inheriting all the attributes and methods of the parent class. 
We use the `super()` function to call the parent class's `__init__` method, and we can override any methods in the child class. 
Here is an example:
```python
class Student(Person):
    def __init__(self, name, age, major):
        super().__init__(name, age)
        self.major = major

    def say_hello(self):
        super().say_hello()
        print("I am a student and my major is " + self.major + ".")

s1 = Student("Bob", 20, "Computer Science")
s1.say_hello()  # prints "Hello, my name is Bob and I am 20 years old. I am a student and my major is Computer Science."
```
In this example, we have an `Animal` class with two attributes, `name` and `species`, and a method, `speak`. 
We also have two subclasses, `Dog` and `Cat`, which inherit from `Animal`. Both subclasses have a constructor that 
calls the `super()` function to initialize the name attribute and set the species attribute to "Dog" or "Cat", respectively. 
The `Dog` and `Cat` classes also override the speak method to print "Woof!" and "Meow!", respectively. 
Finally, we have a function, `animal_speak`, which takes an `Animal` object as a parameter and calls its speak method. 
The `animal_speak` function demonstrates polymorphism, as it can accept objects of different subclasses and call their 
overridden speak methods.

**3. Polymorphism:**

Polymorphism is the ability of different objects to respond to the same message or method call. In Python, we can 
achieve polymorphism through method overriding and duck typing. Here is an example:

```python
class Shape:
    def draw(self):
        pass

class Circle(Shape):
    def draw(self):
        print("Drawing a circle.")

class Square(Shape):
    def draw(self):
        print("Drawing a square.")

class Triangle(Shape):
    def draw(self):
        print("Drawing a triangle.")

shapes = [Circle(), Square(), Triangle()]

for shape in shapes:
    shape.draw()
```

In this example, we have a `Shape` class and three subclasses: `Circle`, `Square`, and `Triangle`. 
Each subclass overrides the draw method to draw a specific shape. We create a list of shapes and call the draw method on 
each shape, which results in the correct shape being drawn for each object in the list.


### Selected examples

**Example 1: Simple creation of a class and an object**
```python
class Animal:
    def __init__(self, name, species):
        self.name = name
        self.species = species
        
    def speak(self):
        print("I am an animal and I can speak!")
        
# Creating an instance of the Animal class
my_animal = Animal("Rex", "Dog")

# Accessing attributes and methods of the instance
print(my_animal.name)      # prints "Rex"
print(my_animal.species)   # prints "Dog"
my_animal.speak()          # prints "I am an animal and I can speak!"
```
Explanation: This code defines a class called `Animal` with a constructor that takes in two parameters, name and species. 
The `__init__` method initializes two instance variables, `self.name` and `self.species`, with the values of the 
parameters passed in. The `Animal` class also has a method called `speak`, which prints a message saying that the 
animal can speak. An instance of the `Animal` class is created with the name "Rex" and species "Dog", and the `name`, `species`, 
and `speak` methods are accessed on that instance.

**Example 2: Inheritance and Polymorphism**

```python
class Animal:
    def __init__(self, name, species):
        self.name = name
        self.species = species
        
    def speak(self):
        print("I am an animal and I can speak!")
        
class Dog(Animal):
    def __init__(self, name, breed):
        super().__init__(name, "Dog")
        self.breed = breed
        
    def speak(self):
        print("Woof!")
        
class Cat(Animal):
    def __init__(self, name, color):
        super().__init__(name, "Cat")
        self.color = color
        
    def speak(self):
        print("Meow!")
        
# Creating instances of the Animal, Dog, and Cat classes
my_animal = Animal("Rex", "Dog")
my_dog = Dog("Buddy", "Golden Retriever")
my_cat = Cat("Whiskers", "Black")

# Accessing attributes and methods of the instances
my_animal.speak()   # prints "I am an animal and I can speak!"
my_dog.speak()      # prints "Woof!"
my_cat.speak()      # prints "Meow!"
```

Explanation: This code defines a base class called `Animal` with a constructor that takes in two parameters, name and species. 
The `Animal` class also has a method called speak that does nothing (because different animals make different sounds). 
The `Dog` and `Cat` classes inherit from the `Animal` class and each override the speak method with their own sound. 
Instances of the `Animal`, `Dog`, and `Cat` classes are created with different names and breeds/colors, and the `speak` 
method is called on each instance, printing out the appropriate sound.

**Example 3: Nested subclasses**

```python
class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        print("I am an animal and I can speak!")

    def eat(self):
        print("I am an animal and I can eat!")

class Mammal(Animal):
    def __init__(self, name, hair_color):
        super().__init__(name)
        self.hair_color = hair_color

    def produce_milk(self):
        print("I am a mammal and I can produce milk!")

    def speak(self):
        print("I am a mammal and I can speak!")

class Primate(Mammal):
    def __init__(self, name, hair_color, is_tool_user):
        super().__init__(name, hair_color)
        self.is_tool_user = is_tool_user

    def use_tools(self):
        if self.is_tool_user:
            print("I am a primate and I can use tools!")
        else:
            print("I am a primate but I cannot use tools!")

    def speak(self):
        print("I am a primate and I can speak!")

class Ape(Primate):
    def __init__(self, name, hair_color, is_tool_user, is_bipedal):
        super().__init__(name, hair_color, is_tool_user)
        self.is_bipedal = is_bipedal

    def walk_bipedal(self):
        if self.is_bipedal:
            print("I am an ape and I can walk bipedally!")
        else:
            print("I am an ape but I cannot walk bipedally!")

    def speak(self):
        print("I am an ape and I can speak!")

# Creating instances of the classes
chimpanzee = Ape("Chester", "black", True, True)
gorilla = Ape("George", "black", False, True)

# Calling methods on the instances
chimpanzee.eat()              # prints "I am an animal and I can eat!"
chimpanzee.produce_milk()     # prints "I am a mammal and I can produce milk!"
chimpanzee.use_tools()        # prints "I am a primate and I can use tools!"
chimpanzee.walk_bipedal()     # prints "I am an ape and I can walk bipedally!"
chimpanzee.speak()            # prints "I am an ape and I can speak!"

gorilla.eat()                 # prints "I am an animal and I can eat!"
gorilla.produce_milk()        # prints "I am a mammal and I can produce milk!"
gorilla.use_tools()           # prints "I am a primate but I cannot use tools!"
gorilla.walk_bipedal()        # prints "I am an ape and I can walk bipedally!"
gorilla.speak()               # prints "I am an ape and I can speak!"

```
Explanation: In this example, we have an `Animal` class which has methods for speak and eat. The `Mammal` class inherits 
from `Animal` and has an additional method `produce_milk`. The `Primate` class inherits from `Mammal` and has an additional 
method `use_tools`. The `Ape` class inherits from `Primate` and has an additional method `walk_bipedal`.

Each class has a speak method, which is overridden in each subclass with a more specific message. The `__init__` methods of each class use 
`super()` to call the parent class's `__init__` method and add any additional  attributes specific to that subclass.

## Live tutorial 

On May 15th 2023, we had a great hands-on example taught by [Rıza Özçelik](https://github.com/rizaozcelik). 

You can watch the tutorial by following [this link](https://drive.google.com/drive/folders/1R3XXT55e0fd_Yj-uARiWz0E3TkbL2RdW?usp=sharing).
You can also download the code and play around with it [here](materials/OOP_code.zip)!

## OOP commands cheatsheet

Here's a selection of main commands for OOP in Python, for your convenience:

| Command                      | Description                                                                                     | Example                                                                      |
|------------------------------|-------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------|
| `class`                      | A keyword used to define a new class.                                                           | `class Animal:`<br>`    def __init__(self, name):`<br>`        self.name = name` |
| `self`                       | A reference to the instance of the class that the method is being called on.                    | `def speak(self):`<br>`    print(f"{self.name} says hi!")`                   |
| `__init__`                   | A special method used to initialize the instance of a class.                                   | `dog = Animal("Fido")`                                                       |
| `super()`                    | A function used to call a method from the superclass in the subclass.                          | `super().__init__(name)`                                                      |
| `@classmethod`              | A decorator used to define a class method that can be called on the class itself.               | `@classmethod`<br>`def num_legs(cls):`<br>`    print(f"{cls.__name__} has 4 legs")` |
| `@staticmethod`             | A decorator used to define a static method that can be called on the class itself.              | `@staticmethod`<br>`def eat():`<br>`    print("yum yum")`                      |
| `@property`                  | A decorator used to define a getter method for a class attribute.                              | `@property`<br>`def name(self):`<br>`    return self._name`                     |
| `@attribute_name.setter`     | A decorator used to define a setter method for a class attribute.                              | `@name.setter`<br>`def name(self, value):`<br>`    self._name = value`         |
| `isinstance()`               | A function used to check if an object is an instance of a certain class.                       | `isinstance(dog, Animal)`                                                     |
| `issubclass()`               | A function used to check if a class is a subclass of another class.                            | `issubclass(Dog, Animal)`                                                     |
| `__str__`                    | A special method that returns a string representation of the object.                                          | `def __str__(self):`<br>`    return f"My name is {self.name} and I have {self.num_legs} legs"` |
| `__repr__`                   | A special method that returns a string representation of the object that can be used to recreate the object. | `def __repr__(self):`<br>`    return f"{self.__class__.__name__}('{self.name}')" `           |
| `__len__`                    | A special method that returns the length of the object.                                                       | `def __len__(self):`<br>`    return len(self.name)`                                          |
| `__getitem__`                | A special method that allows you to access elements of the object using square bracket notation.             | `def __getitem__(self, index):`<br>`    return self.name[index]`                            |
| `__setitem__`                | A special method that allows you to set elements of the object using square bracket notation.                 | `def __setitem__(self, index, value):`<br>`    self.name[index] = value`                   |
| `__delitem__`                | A special method that allows you to delete elements of the object using square bracket notation.              | `def __delitem__(self, index):`<br>`    del self.name[index]`                              |
| `__call__`                   | A special method that allows you to call an object like a function.                                           | `def __call__(self, x):`<br>`    return self.num_legs * x`                                 |
| `hasattr()`                  | A function used to check if an object has a certain attribute.                                                | `hasattr(dog, 'name')`                                                                     |
| `getattr()`                  | A function used to get the value of a certain attribute of an object.                                          | `getattr(dog, 'name')`                                                                     |
| `setattr()`                  | A function used to set the value of a certain attribute of an object.                                          | `setattr(dog, 'name', 'Buddy')`                                                            |
| `delattr()`                  | A function used to delete a certain attribute of an object.                                                    | `delattr(dog, 'name')`                                                                     |


## Additional resources
* [Book] [A Byte of Python -- Object-oriented programming](https://python.swaroopch.com/oop.html):  a free book on programming using the Python language. It serves as a tutorial or guide to the Python language for a beginner audience. 
* [Online tutorial] [Object-Oriented Programming (OOP) in Python 3](https://realpython.com/python3-object-oriented-programming/): step-by-step explanation of OOP for Python 3.
<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>
