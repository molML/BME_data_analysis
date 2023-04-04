---
layout: default
title: Good software principles
parent: Advanced programming
nav_order: 1
---
# Good software principles
{: .no_toc }

Blablablabla something on the fact that there are no rules that are set in stone, but it is good to know what the heck we are doing.
Below you will find several accepted guidelines. 


<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

---


## 1. Keep it Simple, Stupid! (KISS)

KISS (Keep It Simple, Stupid!) is a design principle noted by the U.S. Navy in the [1960s](https://en.wikipedia.org/wiki/KISS_principle#cite_note-TDal-1). 
According to the KISS principle, most systems work best if they are simple rather than complicated. 
Therefore, simplicity should be a key goal in design, while unnecessary complexity should be avoided.

As you code your next big project, ensure your programming is simple and clear to understand. The code should not give 
other human beings (or your future self 😉) difficulties when modifying or changing it.

These are some general guidelines on how to keep your code simple:
* *Keep it small.* Your methods need to be small (e.g., not exceeding 40-50 lines).
* *One-method-at-a-time.* Each method should solve only one problem.
* *Chunk your approach.* Make sure you’ve broken all the conditions you have in down into smaller blocks of codes.

Always Keep It Simple, Stupid (KISS) allows you and fellow programmers to identify bugs quickly. It also helps you modify and make further changes to the code. It is one of the most common lean principles in agile software engineering.


## 4. Don’t Repeat Yourself (DRY)
Don’t Repeat Yourself (DRY) Software Development Principles | Laneways.agency
Source: Think Automation
When writing your code, don’t repeat yourself. That is, avoid copy-pasting your code in different places. Otherwise, future maintenance will be difficult. The reason is that you will have to make changes to the coding in those various places.

Those changes will further necessitate changes in the tests to make the results click green. All of that will need more time, effort, and money.

To avoid such a pitfall, you can extract a common logic into functions.

Additionally, if there are any manual works that you can automate, do so to keep your code lean.

For software development, the above steps will help in the code re-usability without having to repeat it.

We build custom software with modern solutions in mind for any business and sizes!

## 5. Occam's Razor
William Occam was a 14th Century philosopher that coined this principle. It states that in a group of hypotheses, always select the one that has the fewest assumptions.

In keeping up with the Lean Software Development, always start with the most straightforward possible code. Then carefully add the more complex ones only when they’re necessary.

Simple codes allow you to easily envision, develop, test, and correct the product at every step. They also significantly reduce bugs and will enable the program to run faster.

## 6. Big Design Up Front (BDUF)
This software engineering principle affirms that a developer should complete the project’s design first. After that, they can now implement it.

Proponents argue that this helps in discovering issues at the requirements stage and solving them quickly.

However, changes in the software requirements may occur during the project’s life cycle. Such changes may cause difficulties or even render the design code obsolete.

One way to solve this is to have the general architecture first. Then divide the requirements into several stages according to priorities. During the development process, start with the highest to the lowest priority stage. At every step, implement the BDUF principle before the actual coding process.

## 7. Avoid Premature Optimization
Donald Knuth asserted that the root of all evil in programming is premature optimization.

We all agree that optimization speeds up the development process and reduce resource consumption. However, if you do it too early, it may backfire.

Avoid Premature Optimization Software Development Principles Laneways.agency
Source: JS Manifest
The reason is that prioritizing a code is time-consuming and complicated if not done at the right stage. Additionally, when you are implementing the most optimal approach, software requirements may change. If that happens, your program ends up in a dustbin or become difficult to change.

Therefore, start with the easiest approach, even if it is not the most optimal. Then in the future, assess the chosen method in terms of resource and time consumption. Based on your assessment, you can move onto a faster algorithm that consumes fewer resources or efforts.

## 8. Least Astonishment
The principle of least astonishment says that it is advisable to design a feature that doesn’t have a high-astonishment factor.

Your system’s components should behave in a way that end-users expect. Therefore, your project’s outcomes will be profitable only if they are obvious, predictable, and consistent. Otherwise, users will shy from using features or structures that astonish, surprise, or confuse them.

You are making software products for people to use. Thus, you’ll reap a lot by designing user-friendly features. Strive to match human beings’ mental models, experience, and expectations.

Remember, you have to capture the user’s attention as quickly as possible. As we know, the current users’ attention span has plummeted.

## 9. Demeter
The law of Demeter attempts to divide responsibilities between classes and reduce coupling between them. The idea comes from the “only talk to your friends” idiom.

It is highly recommendable to:

» Keep software entities independent of each other. 

» Reduce the communication or coupling between different classes.

» Put related classes in the same package, module or directory to achieve cohesion.

Following this idea allows your application to be more maintainable, understandable, and flexible.

## 10. S.O.L.I.D
It is an acronym that stands for five object-oriented programming and design principles.

» S- Single Responsibility Principle (SRP)

» O- Open/Closed Principle (OCP)

» L- Liskov Substitution Principle

» I-Interface Segregation Principle

» D- Dependency Inversion Principle

S.O.L.I.D Software Development Principles | Laneways.agency
Source: AraGeek
Let’s take a brief look into each of these principles:

Single Responsibility Principle (SRP)

It is a software engineering principle that states that a class should have only one reason to change. In other words, it must have only one responsibility.

Here, we are talking about cohesion. All elements in given class structures or modules should have a functional affinity to one another. By clearly defining your class’s responsibility, you increase its cohesiveness.

Open/Closed Principle (OCP)

The principle says that you should be able to change the behavior of a class without modifying it.

Therefore, you can extend the class’s behavior through composition, interface, and inheritance. However, you cannot open it for minor modifications.

Liskov Substitution Principle (LSP)

In her 1988 research paper, Barbara Liskov stated that derived classes should be replaceable by their base class(es). Thus, you need to exercise care when using inheritance in your project works.

While inheritance is beneficial, it is advisable to use it contextually and moderately. The principle strives to prevent cases where classes are extended only through common things.

You need to consider the pre-conditions and post-conditions of a class before performing inheritance.

Interface Segregation Principle (ISP)

ISP prefers many specific interfaces to a general interface. The goal is to have finely grained and client-specific interfaces.

You need to enhance cohesion in interfaces and develop lean modules- those with few behaviors.

Interfaces that have many behaviors are hard to maintain and evolve. So, you should avoid them.

## 10. Dependency Inversion Principle (DIP)

The principle asserts that programmers should depend on abstractions and not on concrete classes. We can break it into two:

» High-level modules need to be independent of low-level ones. Both should depend on abstractions

» Abstractions should be independent of details. Details should depend on abstractions.

So, what is the reason behind this principle? The answer is that abstractions don’t change a lot. Therefore, you can easily change the behavior of your closed or open-source code. That way, you boost its future evolution.


## Containers and virtual environments



<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>

