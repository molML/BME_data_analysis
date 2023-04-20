---
layout: default
title: Algorithmic complexity
parent: Advanced programming
nav_order: 2
---
# Algorithmic complexity
{: .no_toc }


> *In the world of code and programming,\
There's a measure we use for everything,\
It's algorithm complexity, so vast and grand,\
A way to measure how efficient code can stand.*
> 
> *Big O notation, the first we know,\
Tells us how fast our code can go,\
As input sizes increase and scale,\
Big O helps our code prevail.*
> 
> *Memory complexity, another we need,\
To ensure our code doesn't exceed,\
The resources available to it,\
And cause our software to throw a fit.*
> 
> *But algorithm complexity goes beyond,\
To measure code in another bond,\
Cyclomatic complexity, the count of flow,\
And how many paths our code does show.*
> 
> *With decisions and loops, our code becomes,\
A web of complexity, for some,\
But by understanding its depth and height,\
We can write maintainable code that's just right.*
> 
> -- [ChatGPT](https://chat.openai.com/).


<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>


## Time complexity and the big O
The time complexity of an algorithm is the amount of time it takes to solve a problem, expressed as a function of the size of the input.
This is often captured by the *O* notation ("Big O"). The Big O notation provides an upper bound on the rate of growth of an 
algorithm's runtime as the input size grows. It is commonly used to describe the worst-case scenario for an algorithm, 
but can also be used to describe the best-case and average-case scenarios as well.

In the Big O notation, the runtime of an algorithm is expressed as a function of the input size, typically denoted by *n*. 
For example, an algorithm with a runtime of O(n) means that its runtime grows linearly with the input size, i.e., if the 
input size doubles, the runtime will also double.

Other common Big O notations include:
- *O(1)*: constant time algorithms
- *O(log n)*: logarithmic time algorithms 
- *O(n<sup>2</sup>)*: quadratic time algorithms
- *O(2<sup>n</sup>)* for exponential time algorithms. 

The higher the exponent in the Big O notation, the worse the algorithm's performance becomes as the input size grows.

<img src="https://devopedia.org/images/article/17/4996.1513922020.jpg" width=600>

<sup>Image credits [Devopedia](https://devopedia.org/algorithmic-complexity) </sup>

Understanding the Big O notation is important for developers because it helps them design and choose algorithms that are appropriate for the task at hand. An algorithm with a lower computational complexity will generally be faster and more efficient than an algorithm with a higher computational complexity.

In summary, the Big O notation provides a way to measure and compare the computational complexity of algorithms, which is an important consideration when designing and choosing algorithms for a given task. By understanding the Big O notation, developers can make informed decisions about which algorithms to use to optimize the performance of their software.

## Memory complexity
Memory complexity is a measure of the amount of memory required by an algorithm to solve a problem, as the size of the input data increases. It is a way to describe the space requirements of an algorithm, and is usually measured in terms of the amount of memory required by the algorithm to store and manipulate data.
The memory complexity of an algorithm is often expressed in terms of the amount of memory it requires to store a single data element, multiplied by the size of the input data. For example, an algorithm with a memory complexity of O(n) means that it requires a amount of memory that grows linearly with the size of the input data.
Memory complexity is important because it helps us understand the limitations of an algorithm in terms of the amount of memory required to solve a problem. Algorithms with a high memory complexity may not be able to handle large inputs or may run out of memory on computers with limited resources.
In some cases, memory complexity may also be a limiting factor for performance, as accessing and manipulating large amounts of data in memory can be time-consuming. As such, it is important to design algorithms that minimize their memory requirements whenever possible.

## Cyclomatic complexity
Cyclomatic complexity is a measure of the complexity of a program's control flow. It is based on the number of independent 
paths that can be taken through a program's source code.

The higher the cyclomatic complexity, the more complex the code is likely to be, and the more difficult it can be to test, 
maintain, and modify. Code with a high cyclomatic complexity can also be more prone to bugs and errors, as it can be 
harder to understand and reason about.

Cyclomatic complexity is calculated by counting the number of decision points in a program, such as if statements and 
loops, and adding one to that count. Each decision point represents a branch in the program's control flow, and each 
additional branch increases the complexity of the code.

In mathematical terms, the cyclomatic number (*V(G)*) for a single method or program can be computed as: 

*V(G)* = *E* - *N* + 2
where *E* is the number of edges, and *N* is the number of nodes in the graph. If you're looking at a shortcut on how to 
compute the cyclomatic complexity, have a look at the slides ;) 

This provides a simple way to measure the complexity of a program's control flow and identify areas that may require attention or refactoring to 
improve its readability and maintainability.


<img src="https://craftofcoding.files.wordpress.com/2014/11/cyclo_complexity.jpg" width=600>

<sup>Image credits [CraftofCoding](https://craftofcoding.wordpress.com/2017/06/18/coding-a-small-note-on-cyclomatic-complexity/) </sup>

By measuring cyclomatic complexity, developers can identify areas of their code that may need refactoring or simplification, 
and ensure that their code is easier to test, maintain, and modify over time. It is also a useful tool for evaluating code quality and identifying potential bugs and errors before they occur.


<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>

