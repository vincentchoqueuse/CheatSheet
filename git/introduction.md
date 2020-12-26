# Introduction

## Why Git

### How to Install Git

There are several ways to install Git for your computer \([https://git-scm.com/book/en/v2/Getting-Started-Installing-Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)\). If you have installed Anaconda, you can simply run the following command in your terminal

```text
$ conda install git
```

### How to use Git

There are several graphical interface to use git, however I recommend my students to use classical git command from terminal. A wonderful ressource to learn git is the Pro Git book written by Scott Chacon and Ben Straub and published by Apress.

* [Pro Git Book](https://github.com/progit/progit2/releases/download/2.1.277/progit.pdf)

All the power of git relies on the use of several web plateform for code sharing, reviewing and more. There are basically two options :

* [Github](https://github.com) :  The Github plateform allows you to share, distribute your code. By default, free plan can only create public repo but there are also non-free plans for more specific usage \(private repo, ...\).
* [Gitlab](https://about.gitlab.com/install/) : Gitlab is also quite popular in many tech firms. As compared to Github, Gitlab can be installed on your private server. There is a very high probability that your school or institution has a fully functionnaly git server.

## Snippests

### Initialization

### Push your local change to your distant repo

```text
$ git add .
$ git commit -m "a message explaining your modification"
$ git push -u origin master
```

{% hint style="info" %}
For your projects, I always recommend my student to use a `.gitignore` file to only keep track of their essential files. The content of the gitignore file depends on the programming language used in your project.

* List of [commonly used gitignore files](https://github.com/github/gitignore)
{% endhint %}

