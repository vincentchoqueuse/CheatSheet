# Introduction

* [https://docs.python.org/3/](https://docs.python.org/3/)

### Why Python

Python is a multipurpose interpreted language that provides many packages for scripting, plotting, data science, web developement, and more. Python has a beautiful syntax and is easy to learn. This language has become extremely popular in one decade.

#### How to Install Python

My recommended way to install python on your machine \(whatever your OS\) is to install the Anaconda distribution. This distribution contains many installed package for data science such as Numpy, Scipy, Matplotlib or Jupyter. The Anaconda distribution is quite stable and there is a very small probability that the installation goes wrong with your computer

* [Install Anaconda](https://www.anaconda.com/products/individual#Downloads)

> At the end of the installation process, please make sure to add anaconda in `PATH`.

#### How to use with Python

There are several options to write your code in Python and to run your script. To write your code, the most simple solution is to use a simple text editor. To run your script, you can use your OS terminal. To simplify the process, I recommend to use an IDE such as VScode from Microsoft with the Python Extension.

* [Install VScode](https://code.visualstudio.com)
* [Install Python Extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python)

For teaching, I also recommend my students to use Jupyter Notebook. This web environment allows to add text, equations, python code, figures in a single file. Jupyter is included in the Anaconda Python distribution.

### Control Flow Tools

* [Documentation](https://docs.python.org/3/tutorial/controlflow.html)

#### If statement

```text
x = int(input("Please enter an integer: "))
if x < 0:
    print('lower than 0')
else:
    print('larger or equal to 0')
```

#### For loop

```text
for i in range(5):
    print(i)
```

