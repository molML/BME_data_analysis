---
layout: default
title: Git and version control
parent: Advanced programming
nav_order: 3
---
# Git and version control
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
## About Version Control

Version control is a system that records changes to a file or set of files over time so that you can recall specific 
versions later. Many types of version control exist:

Version control (VC) is a way of tracking changes to files over time, enabling specific versions to be retrieved later. 
There are several types of version control: 
Distributed VCSs, 

1. *Local Version Control Systems*. Local VCSs involve copying files to a directory, but this method is prone to errors. 
It is easy to forget which directory you’re in and accidentally write to the wrong file or copy over files you don’t mean to.
2. *Centralized Version Control Systems (CVCS)*. The next major issue that people encounter is that they need to collaborate with developers on other systems. 
To deal with this problem, Centralized Version Control Systems (CVCSs) were developed. Centralized VCSs have a single 
server that stores all versioned files, with clients checking out files from that central location. For many years this has been the standard.
While this approach offers benefits such as better control and easier administration, it also has a major drawback: if the server fails, collaboration is impossible. 
3. *Distributed Version Control Systems (DVCS)*. VCSs such 
as [Git](https://git-scm.com/about), [Mercurial](https://www.mercurial-scm.org/), [Darcs](http://darcs.net/), or [Bazaar](https://bazaar.canonical.com/en/), 
provide a solution by allowing clients to fully mirror the repository including its 
complete history, rather than simply checking out the latest snapshot of the files. This means that if a server fails 
and the system was collaborating through it, any client repository can be used to restore it. Consequently, every clone 
acts as a complete backup of all the data.

## Git


### Installing Git


## GitHub and GitLab





## References

- [Book] [Pro Git](https://git-scm.com/book/en/v2), S. Chacon and B. Straub, Apress publishing.

<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>

