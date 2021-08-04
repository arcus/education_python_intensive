# Introduction to Python

:::info
## Overview

In this module, learners will become familiar with Python code and why they might want to use it in their research, and practice using Python in a Jupyter notebook. This module is appropriate for a learner at the beginner level.

**Estimated time to completion**: 1 hour

**Pre-requisites**: Learners should be familiar with tabular data (data stored in a rectangular format, like an Excel spreadsheet or a comma separated file). Learners do not need to have access to Python or Juypyter notebooks on their own computers. 

**Learning Objectives**:

After completion of this module, learners will be able to:

* Describe what Python is and why they might want to use it for research
* Download Python and Jupyter using Anaconda
* Recognize Python code

:::

## Content:

- [Preparation](#Preparation) (activity)
- [What is Python?](#So-what-is-Python-anyway) (2 min read)
- [What does Python code look like?](#What-does-Python-code-look-like) (2 min read)
    - [Python scripts](#Python-scripts)
    - [Jupter notebooks](#Jupter-notebooks)
- [Using a Jupyter notebook](#Using-a-Jupyter-notebook) (activity)
    - [(Optional video) Jupyter notebooks](#Optional-video)
- [Next Steps](#Next-steps)(2 min read)
    - [Installing Python on your computer](#Installing-Python-on-your-own-computer) (1 min read)
        - [(Optional video) Installing Python using Anaconda](#Installing-Python-using-Anaconda)
    - [Further reading](#Further-reading)(1 min read)

## Preparation

For the hands-on activities in this module, we will be using an online environment containing a Juypter notebook. To load the environment, open the link below in a new tab:


The environment take a few minutes to load, so be patient. Read through the next couple of sections while you wait! We'll won't need the online environment until the ["Using a Jupyter notebook" section](#Using-a-Jupyter-notebook).

:::success
- [ ] Finished this section? Check it off here!
:::


## So what is Python, anyway?

While the word "python" might immediately make you think of a snake, that's not all it is! Python refers to a programming language. There are a lot of different programming languages for a variety of tasks, but what they all have in common is that they tell your computer what to do. Behind all of your favorite applications is a software developer (or, more often, several developers) who have written the instructions for the computer in a programming language. Python is a particularly versatile language that can be used for web development, data science, machine learning, and more.

So why should you consider Python for your data analysis? There are a few reasons:

- Python is that it is designed to be *human readable*. It's philosophy is centered around producing simple, efficient, easy-to-read code, but you shouldn't get too hung up on that-- code that works for you is good code! Creating human-readable code is great for research because your analyses can be more reproducible (if you know exactly what you did, you can reproduce it) and transparent (writing the methods section of your paper is much easier when you have clear language as to what you did and why).

- Python is free to download and use, and it is an *open source* language, meaning that updates and innovations happen more quickly than proprietary software (to learn more about open source, see **link to open source module**).

- Because Python is quite popular and fairly mature, there are quite a lot of resources out there to help you get started learning, from free online tutorials and cheatsheets to semester-long courses, and everything in between.

Python can be written in several ways. You can write Python code interactively using your computer's Terminal program or Command Line, you can write scripts that include Python code, or you can create Python notebooks using Jupyter or Google Colaboratory (or "Colab" for short). In most cases, you'll need to start with downloading Python to your computer (the exception will be if you are using cloud-based solutions like Google Colab).

:::success
- [ ] Finished this section? Check it off here!
:::

## What does Python code look like?

There are a variety of ways that people write Python code, depending on their goals. If you have Python installed on your computer, you can use your computer's Command Line or Terminal program to write Python code interactively, like this:

![Writing Python code in the terminal](https://github.com/arcus/education_python_intensive/blob/main/images/python-interactive.png?raw=true)

Typing "python3" in the Command Prompt/Terminal opens a Python *interpreter* in interactive mode. This can be a useful tool to check and see if short pieces of code work like you think they do! Most of the time, though, you won't be typing code like this directly in the Terminal. Usually, you'll either be using Python scripts or using a notebook.

### Python scripts

Instead of writing instructions one at a time, for more complex tasks you might want to write a Python script, a series of instructions that you can write out ahead of time and then run in order with one commmand. Programming scripts are often written using special text editors that are designed for writing code (such as Atom or Sublime) or full-featured integrated development environments, or IDEs for short (IDEs, such as PyCharm or Spyder, have more debugging and automation capabilities than text editors). 

Here is a short script written in the Spyder IDE:

![Writing Python in Spyder]()

Spyder has a console, where you can see the output of your script without having to run it in the Command Prompt/Terminal:

![Python output in Spyder]()

### Jupter notebooks

If you are interested in using Python for data analysis, you might want to write Python in a Jupyter notebook (which used to be called an IPython notebook). There are a couple of reasons why you should consider using Jupyter notebooks:

- It is the best of both worlds between interactive and scripted code: code is written in chunks that can be run individually, with any output displayed beneath the code chunk. 
- You can intersperse sections of text, written in Markdown language, that can provide explanations and context for your code. This is especially valuable for data analysis, almost functioning as a scientific notebook.

If you're interested in learning how to write Python code in a Jupyter notebook? Continue on to the next section for a hands-on activity! You won't need to download anything to your computer. 

:::success
- [ ] Finished this section? Check it off here!
:::

## Using a Jupyter Notebook

This is a hands-on activity! If you would prefer to watch a video of the activity, proceed to the [next section](#Optional-video).



:::success
- [ ] Finished this section? Check it off here!
:::

## Next Steps

Are you interested in learning more about Python, or even starting to work with it? Here's what you might want to do next:

### Installing Python on your own computer

Your computer most likely will *not* have Python already installed. To check, you can open your Command Line/Terminal and type `python --version`. The version you have will be displayed if you have Python installed. If you don't, you can go [here](https://www.python.org/downloads/) to download the latest version.

Alternatively, you can install Python using [Anaconda](https://www.anaconda.com/products/individual), a toolkit that gives you not only Python itself but also many other data science tools to help with coding, analysis, and visualization. The individual version of Anaconda is also free to download!

Once you've downloaded Anaconda, you can open the Anaconda Navigator; when you do, you'll see this:

![Anaconda Navigator interface]()

Now you have access to lots of tools for working with Python!

### Further reading

If you want to continue with this Python Intensive Series, or learn a bit more about other data science topics, here are some places to go next:

- [Data Science in Python]()
- [Data Visualization with Python]()
- [Intro to Machine Learning with Python]()
- [Notebooks]()
- [Why Open Source?]()

:::success
- [ ] Finished this section? Check it off here!
:::


