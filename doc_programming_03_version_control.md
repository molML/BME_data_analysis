---
layout: default
title: Git and version control
parent: Advanced programming
nav_order: 3
---
# Git and Version Control
{: .no_toc }


<img src="http://images3.memedroid.com/images/UPLOADED29/5b7d571106c71.jpeg" width=600>

<sup>Image credits [DangerousPizza](https://www.memedroid.com/memes/detail/2465946/Version-control)</sup>

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

In this course, we will be using Git as a DVCS, as it is open-source and community-driven, and offers many options 
for version control. 

## Version control with Git

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Git-logo.svg/1024px-Git-logo.svg.png" width=300>
### What is Git?

Git is a distributed version control system that allows developers to track changes to code and collaborate on 
software projects. Here's how it works:

1. First, developers create a local repository on their own computer. This repository contains all files and folders for the project.
2. As changes are made to the code, developers use Git to create *"commits"*. A commit is a snapshot of the current state 
of the code, along with a brief message describing the changes that were made.
3. Git uses a *"branching"* model to allow developers to work on different features or changes in parallel (*branches*). Each branch is 
a separate copy of the code that can be modified independently.
4. When a developer is ready to share their changes with others, they *"push"* their commits to a remote repository. This 
could be a repository hosted on a web-based Git service like GitHub or GitLab (see [section below](#github-and-gitlab)), 
or it could be a repository hosted on a local server.
5. Other developers can then *"pull"* these changes from the remote repository to their own local repositories. They 
can review the changes and *merge* them into their own branches, resolving any conflicts that arise.
6. Git also includes tools for resolving conflicts and managing code reviews. Developers can leave comments on commits 
and pull requests to discuss changes with other team members.

<img src="https://www.red-gate.com/simple-talk/wp-content/uploads/2020/12/branching-diagram.png" width=700>

<sup>Image credits [red-gate.com](https://www.red-gate.com/simple-talk/devops/database-devops/feature-branches-and-pull-requests-with-git-to-manage-conflicts/)</sup>



Overall, Git provides a powerful set of tools for collaborating on software development projects, while keeping track of 
changes and ensuring that everyone is working on the same code base. It's a critical tool in modern software development 
and is used by millions of developers around the world. You can find detailed info in the official 
[Pro Git](https://git-scm.com/book/en/v2) book. 

### Installing Git
The steps to install Git depend on the operating system you are using. Here are the basic steps for the most common operating systems:

**Windows:**

1. Download the Git for Windows installer from the Git website: https://git-scm.com/download/win
2. Run the installer, following the prompts in the installation wizard.
3. During the installation process, choose the appropriate options for your needs.

Once the installation is complete, open a Command Prompt or Git Bash terminal and verify the installation by running the command `git --version`.

**macOS:**

1. Install Xcode command-line tools by running `xcode-select --install` in the terminal.
2. Install Homebrew package manager by running `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`.
3. Install Git by running `brew install git`.

Verify the installation by running the command `git --version`.

**Linux:**

Open the terminal and use your distribution's package manager to install Git. For example, in Ubuntu, you can run `sudo apt-get install git`.

Verify the installation by running the command `git --version`.

That's it! Once Git is installed, you can start using it in your projects.

If you have additional questions or troubles, refer to the original [Git page](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

### Main Git commands
Here's a list of some of the main Git commands and what they do:

| Command        | Function                                                                                      |
|----------------|-----------------------------------------------------------------------------------------------|
| `git init`     | Initializes a new Git repository in your current directory.                                   |
| `git clone`    | Creates a copy of a Git repository on your local machine.                                     |
| `git add`      | Adds files to the staging area, preparing them for commit.                                    |
| `git commit`   | Commits changes to the local repository, with a message describing the changes.               |
| `git push`     | Uploads local changes to the remote repository.                                               |
| `git pull`     | Downloads changes from the remote repository to your local repository.                        |
| `git status`   | Shows the status of your local repository, including changes to files and the current branch. |
| `git branch`   | Lists all branches in the repository and indicates the current branch.                        |
| `git checkout` | Switches to a different branch.                                                               |
| `git merge`    | Combines changes from one branch into another branch.                                         |
| `git log`      | Displays a log of all commits made in the repository.                                         |
| `git reset`    | Resets the repository to a previous commit.                                                   |
| `git stash`    | Temporarily saves changes that are not ready to be committed.                                 |
| `git tag`      | Creates a tag or label for a specific commit in the repository.                               |

These are just a few of the most commonly used Git commands. There are many more commands and options available depending on your needs and use case, take a 
look at the official [Git website](https://git-scm.com/docs) to get the full list. 💪


### Origin of the name Git
{: .no_toc }

[Hidden bonus paragraph not included in the TOC - congrats, you found it!]

When [Linus Torvalds](https://en.wikipedia.org/wiki/Linus_Torvalds) made his initial commit of Git's code in 2005, he supplied the commit message:

``` Initial revision of "git", the information manager from hell```

In this commit, Linus included a file called README, whose first paragraph reads as follows: 
``` 
GIT - the stupid content tracker

"git" can mean anything, depending on your mood.

 - random three-letter combination that is pronounceable, and not 
   actually used by any common UNIX command.  The fact that it is a
   mispronunciation of "get" may or may not be relevant.
 - stupid. contemptible and despicable. simple. Take your pick from the 
   dictionary of slang.
 - "global information tracker": you're in a good mood, and it actually
   works for you. Angels sing, and a light suddenly fills the room. 
 - "goddamn idiotic truckload of sh*t": when it breaks

This is a stupid (but extremely fast) directory content manager.  It  
doesn't do a whole lot, but what it _does_ do is track directory
contents efficiently.
```
We thought you should know as a good ice-breaker among data scientists 😜

## GitHub and GitLab
GitHub and GitLab are two of the most popular web-based Git repositories used for version control. Both platforms allow 
developers to collaborate on projects, manage code, and track changes to code over time. However, there are some differences between the two platforms.

**GitHub** 

GitHub is a cloud-based Git repository hosting service that provides a graphical user interface (GUI) and a range of 
features such as bug tracking, feature requests, and task management. It is owned by Microsoft and has a large community 
of users. GitHub is primarily used for open source projects, but it also has paid plans for businesses and organizations 
that require private repositories. GitHub has a robust ecosystem of third-party integrations that make it easy to integrate with other tools, such as continuous integration and deployment (CI/CD) services.

<img src="https://allvectorlogo.com/img/2021/12/github-logo-vector.png" width=300>

**GitLab**

GitLab is an open-source Git repository management system that is designed to be self-hosted. It provides a 
web-based GUI that makes it easy to manage Git repositories, track issues, and automate the software development process. 
GitLab has a more comprehensive feature set than GitHub, including code review tools, and issue tracking. 
It also offers a free tier for individuals and small teams, as well as paid plans for businesses and larger organizations.

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e1/GitLab_logo.svg/2560px-GitLab_logo.svg.png" width=300>


Both GitHub and GitLab are excellent tools for version control, but their target audiences differ. 
GitHub is more focused on the needs of the open source community, while GitLab is geared towards businesses and organizations 
that require more advanced features and customizations.




## Resources

- [Book] [Pro Git](https://git-scm.com/book/en/v2), S. Chacon and B. Straub, Apress publishing.
- [Online] [Git and GitHub learning resources](https://docs.github.com/en/get-started/quickstart/git-and-github-learning-resources) online.

<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>

