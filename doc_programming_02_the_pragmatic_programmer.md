---
layout: default
title: Programming pragmatically
parent: Advanced programming
nav_order: 2
---
# Programming pragmatically
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

---
## A Pragmatic philosophy

The expression "Pragmatic Programmer" comes from a [book](https://pragprog.com/titles/tpp20/the-pragmatic-programmer-20th-anniversary-edition/) 
of Dave Thomas and Andy Hunt, who write:
> *"it's an attitude, a style, a philosophy of approaching problems and their solutions. They think beyond the immediate problem,
always trying to place it in its larger context, always trying to be aware of the bigger picture.
After all, without this larger context, how can you be pragmatic? How can you make
intelligent compromises and informed decisions?"*

In what follows, we have identified a few characteristics that will allow you to write better code, in a pragmatical way. These are all based on [The Pragmatic Programmer](https://pragprog.com/titles/tpp20/the-pragmatic-programmer-20th-anniversary-edition/) 
book, where you will find more in-depth insights. 

### Software entropy and the broken window theory

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
Although there are other factors that could cause software decay, neglect is the leading contributor to its acceleration.\
**Don't allow entropy to triumph.**


### Good-enough software

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

## Developing code in an imperfect world

## References

* [Book]    [The Pragmatic Programmer](https://pragprog.com/titles/tpp20/the-pragmatic-programmer-20th-anniversary-edition/). D. Thomas, 
A. Hunt. Ed: Addison-Wesley Professional. 

<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>

