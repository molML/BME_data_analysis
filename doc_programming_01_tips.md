---
layout: default
title: Tips for building reliable programs
parent: Advanced programming
nav_order: 1
---
# Tips for building reliable programs
{: .no_toc }


> *Programming is a craft. At its simplest, it comes down to getting a computer to do what you
want it to do (or what your user wants it to do). As a programmer, you are part listener, part
advisor, part interpreter, and part dictator. [...] What's more, you try to do all this against the relentless ticking
of the project clock.* \
> *You work small miracles every day. It's a difficult job.*
> 
> A. Hunt, D. Thomas - The Pragmatic Programmer.


<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

## Building reliable programs

Developing reliable programs is important in data analysis because it ensures accurate and trustworthy results. Unreliable 
programs can lead to errors and inconsistencies in data analysis, which can undermine the credibility of the results. Reliable 
programs also help to increase efficiency and save time, allowing analysts to focus on insights and decision-making rather 
than debugging and fixing errors. Additionally, reliable programs can help maintain the reputation of analysts and organizations, 
which is important in building and retaining trust among clients and stakeholders.

A reliable program is:

- Modular – you can break it into pieces and test each piece separately.
- Robust – nonsensical input will cause it to fail in a predictable way.
- Deterministic – if it fails, you can easily make it fail in the same way again.
- Testable – you can look inside and understand why it’s doing what it does. 

In what follows, we will give you some tips on how to build programs that are as reliable as possible. 

## Four tips for building reliable programs

### Tip 1. Pay attention to algorithm design
<details close markdown="block">
  <summary>
    Expand
  </summary>

<img src="https://image.jimcdn.com/app/cms/image/transf/dimension=4000x3000:format=png/path/s29986025e909bb6f/image/i41a39f035fa11d70/version/1641979489/enough-design-upfront-vor-big-design-upfront.png" width=600>

<sup>Image credits [Agile Agreement](https://www.agileagreement.com/2020/07/21/enough-design-upfront-vor-big-design-upfront/)</sup>

Algorithm design is important because it determines how efficiently and accurately a program solves a problem. A well-designed 
algorithm can reduce the time and resources required to complete a task, improve the quality of results, and make programs more 
reliable and robust. In contrast, a poorly designed algorithm can result in errors, slow down program execution, and waste resources. 
Effective algorithm design involves understanding the problem requirements, choosing appropriate data structures and algorithms, 
and optimizing the algorithm for performance and accuracy. By focusing on algorithm design, developers can create more efficient 
and effective programs that provide better outcomes for users.

When it comes to algorithm design, there are many 'flavours' of it, that vary in terms of the level of planning and documentation involved:

**1. NDUF** (No Design Up Front).

NDUF is an approach to software development that focuses on creating software through a 
process of continuous iteration and feedback. This methodology is often used in Agile software development, 
where the emphasis is on delivering working software quickly and making changes in response to feedback.

Advantages:
   - Allows for flexibility and adaptation to changing requirements
   - Can be more efficient in delivering working software quickly
   - Can encourage collaboration and communication among team members

Disadvantages:
- May result in incomplete or inconsistent documentation
- Can lead to technical debt or code that is difficult to maintain over time
- May require more effort to ensure overall project cohesiveness

**2. EDUF** (Exploratory Design Up Front) 

EDUF is an approach that involves creating a high-level design for the software before 
development begins. This design is then used to guide the development process, with modifications made as necessary based 
on feedback and testing.

Advantages:
- Provides a clear plan for software development
- Can help identify potential issues early in the development process
- Allows for more efficient use of resources

Disadvantages:
- May lead to rigidity in the development process
- Can result in over-emphasis on planning and documentation rather than actual development
- May not be well-suited for projects with rapidly changing requirements

**3. BDUF** (Big Design Up Front) 

BDUF is an approach that involves creating a detailed design for the software before development 
begins. This design is then used to guide the development process, with little deviation from the original plan.

Advantages:
- Provides a comprehensive and detailed plan for software development
- Can help identify potential issues early in the development process
- Can ensure consistency in the development process

- Disadvantages:
- May lead to inflexibility in responding to changes in requirements
- Can result in over-emphasis on planning and documentation rather than actual development
- Can be time-consuming and resource-intensive

NDUF, EDUF, and BDUF each have their own set of advantages and disadvantages. The choice between these methodologies depends on the specific needs of the project and the team's preferences and capabilities. NDUF and EDUF are generally more suitable for projects with changing requirements, while BDUF is more suitable for projects with well-defined requirements that require a high level of planning and documentation.

</details>

### Tip 2. Keep it Simple, Stupid! (KISS)

<details close markdown="block">
  <summary>
    Expand
  </summary>

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

</details>

### Tip 3. Test, debug, test (again!)

<details close markdown="block">
  <summary>
    Expand
  </summary>

Testing and debugging are both essential parts of the software development process, which should always considered when writing code:

- *Testing* is the process of verifying that a piece of code works as expected. It involves running the code with a variety 
of inputs and checking that it produces the correct output. The purpose of testing is to catch errors early in the development process, 
before the code is deployed to users. Testing can be done manually, where a person manually tests the code, or automated, where 
a software tool is used to run tests automatically.
- *Debugging* is the process of finding and fixing errors in code. When a program doesn't work as expected, debugging helps 
identify the cause of the problem and make necessary changes to fix it. Debugging involves analyzing the code line-by-line 
to find where the error occurred and then making changes to the code to fix it. Debugging can be done with the help of a 
debugging tool or manually by adding print statements to track the code's execution.

Here are a few tips for you, to help test and debug your code
1. Always plan for debugging in your development process.
2. Test early and often. It helps to catch errors early in the development process and reduces the chances of bugs making their way into the final product. Test frequently, ideally after every major change.
3. Use automated testing tools if necessary. Automated testing tools can help streamline the testing process and catch errors more efficiently. 
Tools such as [pytest](https://docs.pytest.org/en/7.3.x/) and [unittest](https://docs.python.org/3/library/unittest.html) can be used to automate testing.
4. Break your code into manageable pieces: Breaking your code into smaller, manageable pieces makes it easier to debug and test. Modular code design helps to minimize the impact of errors, making them easier to detect and fix.
5. Don't assume anything. Don't assume that your code works as intended. Instead, test it and verify that it produces the expected results.

</details>

### Tip 4.Write code for your future self


<details close markdown="block">
  <summary>
    Expand
  </summary>

Writing code for one's future self is an important practice that can save time, reduce errors, and make software easier to maintain. 
Here are a few reasons why writing code with your future self in mind is so important:
- Code is often revisited: In most software projects, code is not written once and forgotten. Instead, it is often revisited 
multiple times for updates, bug fixes, or new features. When you write code with your future self in mind, you are creating a more efficient, effective workflow for your future self to work with.
- Reducing cognitive load: When we write code, we often do it in a way that makes sense to us at the time. However, 
when we revisit that code weeks, months, or even years later, we may have trouble remembering what we were thinking at the time. By writing code that is easy to read and understand, you are reducing the cognitive load on your future self.
- Saving time: By writing clean, modular, and well-documented code, you can save time in the long run. When you need to make
updates or add new features, you can easily find the code you need and understand how it works. This can save you time in the long run and prevent unnecessary delays.
- Easier collaboration: If you are working on a project with others, writing code with your future self in mind can also
make it easier for your teammates to work with. By making your code more readable and understandable, you are reducing the chances of misunderstandings and errors.


<img src="https://cdn.vox-cdn.com/thumbor/iXlaC9fjNJ0XBV3t7_qNLBKBol8=/148x0:1768x1215/1200x800/filters:focal(148x0:1768x1215)/cdn.vox-cdn.com/uploads/chorus_image/image/46650366/bttf.0.0.png" width=600>

Overall, writing code with your future self in mind is a good habit to develop. By doing so, you can create more efficient, maintainable, and effective software that will save you time and effort in the long run.

</details>

## Additional considerations: Programming pragmatically

The expression "Pragmatic Programmer" comes from a [book](https://pragprog.com/titles/tpp20/the-pragmatic-programmer-20th-anniversary-edition/) 
of Dave Thomas and Andy Hunt, who write:
> *"it's an attitude, a style, a philosophy of approaching problems and their solutions. They think beyond the immediate problem,
always trying to place it in its larger context, always trying to be aware of the bigger picture.
After all, without this larger context, how can you be pragmatic? How can you make
intelligent compromises and informed decisions?"*

In what follows, we have identified a few characteristics that will allow you to write better code, in a pragmatical way. These are all based on [The Pragmatic Programmer](https://pragprog.com/titles/tpp20/the-pragmatic-programmer-20th-anniversary-edition/) 
book, where you will find more in-depth insights. 

### Software entropy and the broken window theory

<details close markdown="block">
  <summary>
    Expand
  </summary>


Like the well-known concept in physics, also software can experience entropy. 
The excessive increase of disorder in a piece of software is often referred to as "[software rot](https://en.wikipedia.org/wiki/Software_rot)".

Despite plans and efforts, a project can experience ruin and decay. Yet there are other
projects that, despite enormous difficulties, complexity and constant setbacks, still manage to not rot. 
What makes the difference?

**The broken window theory.** The state of buildings in urban areas can vary greatly, with some being well-maintained and aesthetically pleasing, 
while others are decaying. The reason for this discrepancy has been explored by experts in the field 
of urban decay and crime, who have uncovered a fascinating catalyst that can rapidly lead to the destruction and 
abandonment of a once-inhabited building -- *a broken window*. When a broken window is left unrepaired for an extended 
period, it can create a feeling of neglect among the building's occupants. 
This can lead to a perception that the authorities responsible for the building don't care about its upkeep. 
As a result, other windows may get broken, littering may occur, and graffiti may appear, eventually causing severe structural damage. 
In a short span of time, the owner may lose interest in repairing the building, and the initial perception of neglect becomes an undeniable reality.

The "Broken Window Theory" has inspired Police departments in large cities to address small issues and minor offenses
to prevent serious crime by addressing minor offenses. This approach has proven successful in practice as cracking down 
on small infractions such as broken windows and graffiti has led to a decrease in major crimes.

<p align="center">
<img src="https://img.rawpixel.com/s3fs-private/rawpixel_images/website_content/px855684-image-kwyo946a.jpg?w=800&dpr=1&fit=default&crop=default&q=65&vib=3&con=3&usm=15&bg=F4F4F3&ixlib=js-2.2.1&s=314279ca4d66375ffbe75e40ec35db27" width=450>
</p>

The "Broken Window Theory" also applies to software. Repair every "broken window," whether it be a flawed design, incorrect decision, 
or subpar code, as soon as it's identified. In case there's inadequate time to fix it properly, consider boarding it up. 
A possible solution could be to comment out the faulty code, exhibit a "Not Implemented" message, or replace it with dummy data. 
Taking prompt action will prevent further damage and convey your proactivity in resolving issues. Neglecting to fix these
"broken windows" could lead to a rapid deterioration of an otherwise clean and functional system. 
Although there are other factors that could cause software decay, neglect is the leading contributor to its acceleration.

**...Don't allow entropy to triumph.**

</details>

### Good-enough software
<details close markdown="block">
  <summary>
    Expand
  </summary>

> *Perfect Python software, so elusive and rare,\
A goal we all strive for, yet it's never quite there.\
Bugs and errors, they crop up with ease,\
As we try to make our code work with expertise.*
>
>*We spend hours debugging, fixing and tweaking,\
Hoping for a result that's flawless and speaking,\
To the needs of our users, who expect nothing less,\
But perfection is fleeting, and we must confess,\
That the pursuit of it is what drives us ahead,\
To make software that's better than what we had.*
> 
> Poem written by [ChatGPT](https://openai.com/blog/chatgpt).


Accept that perfect software does not exist. 
In his [seminal paper](https://ieeexplore.ieee.org/abstract/document/382191), Ed Yourdon suggested that programmers can strive to produce software 
that meets the needs of users, future maintainers, and themselves, without necessarily striving for *absolute perfection* but rather
finding a trade-off that is "good enough". This approach<sup>*</sup> can lead to increased productivity, and more effective 
software, as shorter development periods can facilitate more frequent feedback from users.

1. *Involve users in the trade-off.* Always ask yourself how good is good for the envisioned community of users and the 
problem you are tackling. People often would rather use code with some rough edges today than wait a year for the hyper-refined version.
So, don't be a perfectionist and publish your GitHub repo! If you give your users something to play with early, their feedback
will often lead you to a better final version.
2. *Know When to Stop.* It is better to resist the temptation to over-embellish or refine a well-designed program. Instead, 
it can be beneficial to allow the code to speak for itself and exist independently for a time, even if it is not perfect.
It's natural to want to perfect our work, but sometimes it's best to move on and trust in the inherent strength of the software. Don't worry: it
could never be perfect.
3. *Accept that we live an imperfect world* and act accordingly when writing your code. See the 
[Developing code in an imperfect world](#developing-code-in-an-imperfect-world) section below.

<sup>*</sup> <u>NB!</u> The concept of "good enough" does not rule out the quality, reliability and functionality of the produced code, as well as the
requirements of the users/problem at hand. 

</details>

## References
* [Book]    [The Pragmatic Programmer](https://pragprog.com/titles/tpp20/the-pragmatic-programmer-20th-anniversary-edition/). D. Thomas, 
A. Hunt. Ed: Addison-Wesley Professional. 

<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>

