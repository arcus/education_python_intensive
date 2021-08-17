<!--

author:   Meredith Lee
email:    leemc@chop.edu
version:  0.0.1
language: en
narrator: UK English Female
title: Introduction to Python

comment:  This module introductions the Python programming language and demonstrates how to write Python code in the Jupyter notebook.

-->

# Introduction to Python

Welcome to Introduction to Python!

![Python logo](https://github.com/arcus/education_python_intensive/blob/main/images/python-logo-master-v3-TM-flattened.png?raw=true)

## Overview

In this module, learners will become familiar with Python code, explore why they might want to use it in their research, and practice using Python in a Jupyter notebook. This module is appropriate for a learner at the beginner level.

**Estimated time to completion**: 30 min

**Pre-requisites**: Learners should be familiar with tabular data (data stored in a rectangular format, like an Excel spreadsheet or a comma separated file). Learners do not need to have access to Python or Jupyter notebooks on their own computers.

**Learning Objectives**:

After completion of this module, learners will be able to:

* Describe what Python is and why they might want to use it for research
* Recognize Python code
* Write text in Markdown and simple code in a Jupyter notebook
* Download Python using the Anaconda distribution


## Content:

- [Preparation](#Preparation) (2 min activity)

- [What is Python?](#So-what-is-Python-anyway) (2 min read)

- [What does Python code look like?](#What-does-Python-code-look-like) (3 min read)

    - [Python scripts](#Python-scripts) (3 min read)

    - [Jupter notebooks](#Jupter-notebooks) (2 min read)

- [Using a Jupyter notebook](#Using-a-Jupyter-Notebook) (10 min activity)

- [Next Steps](#Next-Steps) (2 min read)

    - [Installing Python on your computer](#Installing-Python-on-your-own-computer) (1 min read)

        - [(Optional video) Installing Python using Anaconda](#Installing-Python-using-Anaconda)

    - [Further reading](#Further-reading)(1 min read)

## Preparation

For the hands-on activity in this module, we will be using an online environment containing a Juypter notebook. To load the environment, open the link below in a new tab:

 **Click here!**
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/arcus/education_python_intensive/main?filepath=intro-to-python.ipynb)

The environment takes a few minutes to load, so be patient. Read through the next couple of sections while you wait! We won't need the online environment until the ["Using a Jupyter notebook" section](#Using-a-Jupyter-notebook).


## So what is Python, anyway?

While the word "python" might immediately make you think of a snake, that's not all it is! Python refers to a programming language. There are a lot of different programming languages for a variety of tasks, but what they all have in common is that they tell your computer what to do. Behind all of your favorite applications is a software developer (or, more often, several developers) who have written the instructions for the computer in a programming language. Python is a particularly versatile language that can be used for web development, data science, machine learning, and more.

So why should you consider Python for your data analysis? There are a few reasons:

- Python is designed to be *human readable*. Its philosophy is centered around producing simple, efficient, easy-to-read code, but you shouldn't get too hung up on that- code that works for you is good code! Creating human-readable code is great for research because your analyses will be more reproducible (if you know exactly what you did, you can reproduce it) and transparent (writing the methods section of your paper is much easier when you have clear language as to what you did and why).

- Python is free to download and use, and it is an *open source* language, meaning that updates and innovations happen more quickly than proprietary software (to learn more about open source, see [this module about open-source software](https://liascript.github.io/course/?https://raw.githubusercontent.com/arcus/education_r25/main/objective_3_1/why_open_source/README.md?token=AQSA4RB2DMZ6EEYYRSJ3VSLBEVGES#1)).

- Because Python is quite popular and fairly mature, there are quite a lot of resources out there to help you get started learning, from free online tutorials and cheatsheets to semester-long courses, and everything in between.

Python can be written in several ways. You can write Python code interactively using your computer's Terminal program or Command Line, you can write scripts that include Python code, or you can create Python notebooks using Jupyter or Google Colaboratory (or "Colab" for short). In most cases, you'll need to start with downloading Python to your computer (the exception will be if you are using cloud-based solutions like Google Colab).

### Knowledge Check

What are some reasons to consider using Python for data analysis? Select all that apply.

[[X]] Python is free and open-source.
[[ ]] Python is simple point-and-click software.
[[X]] Python is human-readable.
[[X]] The Python community has lots of resources to help you get started.

### Knowledge Check

While Python is human-readable and free, it is not point-and-click software, and it can take some time and effort to learn how to write Python code. Don't worry, there are lots of resources out there to help you learn!

## What does Python code look like?

There are a variety of ways that people write Python code, depending on their goals. If you have Python installed on your computer, you can use your computer's Command Line or Terminal program to write Python code interactively, like this:

![Writing Python code in the Terminal](https://github.com/arcus/education_python_intensive/blob/main/images/python-interactive.png?raw=true)

Typing "python3" in the Command Prompt/Terminal opens a Python *interpreter* in interactive mode. This can be a useful tool to check and see if short pieces of code work like you think they do! Python code can be as simple as `7 + 8`. If you type that in the interactive Python interpreter, Python will evaluate the expression and return the value `15`.

Python also has certain functions, code that performs a certain task and returns a certain value, built into it. For example the `print()` function takes an object (such as a string of text or a file) and prints the string to the screen. The code `print("Hello World!")` will return "Hello World!" to the screen. There are a variety of built-in functions. The following code uses two functions to create a list of numbers between 0 and 10:

`list(range(0,10))`

The Python interpreter evaluates expressions from the inside out. The function `range()` generates an immutable  sequence of numbers, including the first number listed but *excluding* the second number. The `list()` function then takes that sequence and converts it to a list of numbers that can be displayed. So the code above would return:

`[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]`

Most of the time, you won't be typing code like this directly in the Terminal. Usually, you'll either be using Python scripts or using a notebook.

### Python scripts

Instead of writing instructions one at a time, for more complex tasks you might want to write a Python script, a series of instructions that you can write out ahead of time and then run in order with one command. Scripts are often written using special text editors that are designed for writing code (such as Atom or Sublime) or full-featured integrated development environments, or IDEs for short (IDEs, such as PyCharm or Spyder, have more debugging and automation capabilities than text editors).

Here is a short script written in the Spyder IDE:

![Writing Python in Spyder](https://github.com/arcus/education_python_intensive/blob/main/images/python-in-spyder.png?raw=true)

In the above example, our script asks for input of a user's name using the `input()` function, stores that input in a variable we've called `name`, and prints out a welcome message to the screen that includes the name the user entered using the code

`print("Welcome to Intro to Python, "+name+"!")`

The Spyder IDE has a console where you can see the output of your script without having to run it in the Command Prompt/Terminal:

![Python output in Spyder](https://github.com/arcus/education_python_intensive/blob/main/images/python-spyder-console.png?raw=true)

As you can see in the screenshot of the console, all we had to do was create the file one time and then run that file instead of typing in the code interactively. This can save you time and effort if you have a task you know you'll want to do over and over again. In the Spyder IDE there is a "run" button (a green arrow in menu at the top) but you could also run the same file in your Terminal/Command Line by typing the command `python` followed by the file name of your Python script. When you save a Python script, you'll use the file extension .py, and so to run the script in the example above, I would navigate to the correct directory in the Terminal (the folder where you've saved your file) and type this:

`python intro-to-python.py`

If you are in the right place, you should see the output of your code!

### Knowledge Check

Which of the following is *not* an example of Python code?

[( )] `print("Python is the best!")`
[(X)] `print Hello World!`
[( )] `list(range(1, 100))`
[( )] `height = input("How tall are you?")`

### Knowledge Check

The Python language uses functions that contain instructions that tell the computer what it is supposed to do, and these functions are the name of the function followed by the *arguments* in parentheses. Arguments are information that the person writing the code (you!) provide to tell the function what data to perform its task on and more specificity on how exactly to perform the task. `print()`, `list()`, `range()`, and `input()` are just a few of Python's built-in functions! You can read more about Python's built-in functions [here](https://docs.python.org/3/library/functions.html).


### Jupyter notebooks

If you are interested in using Python for data analysis, you might want to write Python in a Jupyter notebook (which was previously called an IPython notebook). There are a couple of reasons why you should consider using Jupyter notebooks:

- It is the best of both worlds between interactive and scripted code: code is written in chunks that can be run individually, with any output displayed beneath the code chunk.
- You can intersperse sections of text, written in Markdown language, that can provide explanations and context for your code. This is especially valuable for data analysis, almost functioning as a scientific notebook.

Interested in learning how to write Python code in a Jupyter notebook? Continue on to the next section for a hands-on activity! You won't need to download anything to your computer.


## Using a Jupyter notebook

This is a hands-on activity! Feel free to pop over to that tab you opened in the [Preparation section](#Preparation) to get started. Need the link again? Here it is:

**Click here!**
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/arcus/education_python_intensive/main?filepath=intro-to-python.ipynb)

If you would prefer to watch a video of the activity, or simply want to see a demonstration, we have one here:

**Video coming soon!**

### Knowledge Check 1

What are the components of a Jupyter notebook? Select all that apply.

[[X]] Code cells
[[X]] Text cells written in Markdown
[[ ]] A console where you can write lines of code interactively

### Knowledge Check 1
Jupyter notebooks contain code cells and text cells.

The code cells are written in Python and can contain as much or as little code as you want; the output of the code can be displayed directly beneath the code cell and the code can be edited and re-run at any time.

The text cells are written in Markdown language and can provide more context and reasoning than can easily be done using comments. Additionally, using Markdown allows you to add useful formatting to your text.

Jupyter notebooks do not have console, but since you can run each code cell independently, you don't really need one!

### Knowledge Check 2

How would you refer to the column "age" in a data frame called "students"?

[( )] `age`
[(X)] `students["age"]`
[( )] `students.age()`
[( )] `students[age]`

### Knowledge Check 2
To refer to a column within a data frame, you use the syntax `dataframe["column"]` (don't forget the quotes!). Just `age` by itself would tell Python tp look for a variable called "age". `students.age` would indicate to Python that you wanted to invoke a method `age` on the "students" data frames.


## Next Steps

Are you interested in learning more about Python, or even starting to work with it? Continue on for tips on what you might want to do next!

### Installing Python on your own computer

Your computer most likely will *not* have Python already installed. To check, you can open your Command Line/Terminal and type `python --version`. The version you have will be displayed if you have Python installed. If you don't, you can go [here](https://www.python.org/downloads/) to download the latest version.

Alternatively, you can install Python using [Anaconda](https://www.anaconda.com/products/individual), a toolkit that gives you not only Python itself but also many other data science tools to help with coding, analysis, and visualization. The individual version of Anaconda is also free to download!

Once you've downloaded Anaconda, you can open the Anaconda Navigator; when you do, you'll see this:

![Anaconda Navigator interface](https://github.com/arcus/education_python_intensive/blob/main/images/anaconda.png?raw=true)

Now you have access to lots of tools for working with Python!

### Knowledge Check

How can you access Python to start to practice on your own?

[( )] By downloading the latest version at https://www.python.org/downloads/
[( )] By downloading the latest Anaconda distribution
[( )] By using cloud-based tools, such as Google Colab
[(X)] All of the above

### Knowledge Check
You can download Python directly to your computer, use Anaconda to download Python as well as many other data science tools, or use cloud-based notebooks like Google Colab-- the choice is yours!

### Further reading

If you want to continue with this Python Intensive Series, or learn a bit more about other data science topics, here are some places to go next:

- Data Science in Python (coming soon!)
- Data Visualization with Python (coming soon!)
- Intro to Machine Learning with Python (coming soon!)
- Notebooks (coming soon!)
- [Why Open Source?](https://liascript.github.io/course/?https://raw.githubusercontent.com/arcus/education_r25/main/objective_3_1/why_open_source/README.md?token=AQSA4RB2DMZ6EEYYRSJ3VSLBEVGES#1)
