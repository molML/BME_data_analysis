---
layout: default
title: Virtual environments
parent: Getting started
nav_order: 2

---


# Virtual environments
{: .no_toc }


<p align="center">
<img src="https://files.realpython.com/media/Python-Virtual-Environments_Watermarked.4c787192d42f.jpg" width=500>
</p>
<sup>Image credits [Real Python](https://realpython.com/python-virtual-environments-a-primer/)</sup>

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

## Package dependencies and virtual environments

Python is a powerful programming language that offers a wide range of packages and libraries that can be used to create 
complex applications and solutions. However, as your Python projects grow in size and complexity, you will inevitably 
encounter dependencies between packages. In other words, some packages you use may depend on other packages to 
function correctly. Managing these dependencies can quickly become a challenge, especially when you work on multiple 
projects or collaborate with others. This is where virtual environments come into play. Virtual environments in 
Python provide a way to isolate the packages you use for each project, so you can manage dependencies independently 
and avoid conflicts. By creating a separate virtual environment for each project, you can ensure that you are 
using the correct versions of packages and avoid version conflicts.

<p align="center">
<img src="https://www.researchgate.net/profile/Tim-Evans-2/publication/335564976/figure/fig3/AS:798704449638400@1567437388116/Figure-E5-The-dependencies-of-python-packages-on-one-of-the-authors-machines-in-2019.png" width=500>
</p>

<sup>A true depiction of dependencies of Python Packages. Image from [Vasiliauskaite and Evans](https://arxiv.org/abs/1908.11818)</sup>

## Virtual environments
Virtual environments in Python are isolated environments that allow you to install and manage Python packages without 
affecting the global Python installation. This means you can have multiple Python projects on the same machine with 
different package dependencies, and each project can have its own isolated environment with its own set of packages. 
Virtual environments are essential for managing dependencies and avoiding conflicts between different projects. They 
also make it easier to share code and collaborate with others since you can easily recreate the same environment on 
different machines. Overall, virtual environments are a crucial tool for Python developers to manage dependencies and 
ensure their projects are reproducible and maintainable.

In this course, the usage of virtual environments is highly recommended to ensure:
- Isolation: Virtual environments provide a way to isolate dependencies and package installations for each project. This helps to prevent conflicts between different projects and ensures that each project has access to the required versions of packages and libraries.
- Reproducibility: By using virtual environments, you can create a reproducible development environment for each project. This means that if you share your code with others, they can easily recreate the same environment on their own machines, ensuring that the code runs correctly.
- Flexibility: With virtual environments, you can easily switch between different versions of Python and packages as needed for each project. This makes it easier to experiment with different tools and libraries without affecting your global Python installation.

[Conda](https://docs.conda.io/en/latest/) is recommended as a tool to set up virtual environments, although this can also be done natively in Python, see below.

### Native python environments
You can use the built-in venv module to create a virtual environment for your project. 
Open a command prompt or terminal window, navigate to the directory where you want to create the virtual environment, 
and enter the following command:

```
python -m venv myenv
```
This command creates a new virtual environment named "myenv" in the current directory.

Activate the virtual environment by running the appropriate activation command for your operating system. On Windows, the command is:
```
myenv\Scripts\activate.bat
```
On macOS and Linux, the command is:

```
source myenv/bin/activate
```

When the virtual environment is activated, the command prompt or terminal window will display the name of the virtual 
environment in parentheses, indicating that you are now working within the virtual environment.

Install the packages you need for your project using pip. For example, you can install the requests package by entering 
the following command:
```
pip install requests
```

When you're finished working in the virtual environment, you can deactivate it by entering the following command:
```
deactivate
```
This will return you to your system's default Python installation

### Conda environments (recommended)

[Conda](https://conda.io/) is an open-source package management system and environment management system that makes it easy to install, 
run, and manage software packages and dependencies. It was originally developed to support the data science community, 
but it has since been adopted by developers and researchers in many other fields as well. Conda provides a cross-platform, language-agnostic package manager that can be used to install packages and libraries 
for many different programming languages, including Python, R, and C++. It also provides a flexible environment management
system that allows you to create and manage virtual environments for each project, with specific versions of packages 
and dependencies.


<p align="center">
<img src="https://docs.conda.io/en/latest/_images/conda_logo.svg" width=500>
</p>


To get started with Conda environments, you need to install Conda on your machine. You can download and install Conda from the [official website](https://conda.io/projects/conda/en/latest/user-guide/install).
Once you have Conda installed, you can use it to create a virtual environment. 
Open a command prompt (Anaconda Prompt in Windows recommended) or terminal window, navigate to the directory where 
you want to create the virtual environment, and enter the following command:

```
conda create --name myenv
```

This command creates a new virtual environment named "myenv". Activate the virtual environment by running the following command:
```
conda activate myenv
```

When the virtual environment is activated, the command prompt or terminal window will display the name of the virtual 
environment in parentheses, indicating that you are now working within the virtual environment.

Install the packages you need for your project using Conda. For example, you can install the numpy package by entering 
the following command:
```
conda install numpy
```
You could also use
```
pip install numpy
```
**Note!** We recommend to be careful with mixing the command ```conda install``` with ```pip install``` within a certain
environment, as it might create dependency conflicts. Use either one as consistently as possible.

When you're finished working in the virtual environment, you can deactivate it by entering the following command:
```
conda deactivate
```
This will return you to your system's default Python installation.


## Additional resources
* [Conda user guide] [Managing Environments:](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) conda official page
on how to use environments. 
* [Real Python] [Python Virtual Environments: A Primer](https://realpython.com/python-virtual-environments-a-primer/), a tutorial 
on how to set up and utilize Python virtual environments at their best.


<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>
