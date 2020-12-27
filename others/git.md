# Git

## Why Git

### How to Install Git

There are several ways to install Git for your computer \([https://git-scm.com/book/en/v2/Getting-Started-Installing-Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)\). If you have installed Anaconda, you can simply run the following command in your terminal

```text
$ conda install git
```

### How to use Git

There are several graphical interface to use git, however I recommend my students to use classical git command from terminal. A wonderful ressource to learn git is the Pro Git book written by Scott Chacon and Ben Straub and published by Apress.

* [Pro Git Book](https://github.com/progit/progit2/releases/download/2.1.277/progit.pdf)

All the power of git relies on the concept of distant repo that can be used by many users  for code sharing, reviewing and more. Distant repos are managed by a web plateformThere are basically two options :

* [Github](https://github.com) :  The Github plateform allows to share and distribute your code. By default, free plan can only create public repo but there are also non-free plans for more specific usage \(private repo, ...\).
* [Gitlab](https://about.gitlab.com/install/) : As compared to Github, Gitlab can be installed on a private server. There is a very high probability that your school or institution has a fully functionnaly git server.

## Code Snippest

### Initialization

```text
$ git init
$ touch README.md
$ touch .gitignore
```

I always recommend my students to use a `.gitignore` file to only keep track of their essential files. The content of the gitignore file depends on the programming language used in your project. A list of commonly used .gitigore file can be found below

* [commonly used gitignore files](https://github.com/github/gitignore)


### Push your local changes to your distant repo

The three following commands show how to push your changes from your local machine to your `master` branch of your distance repo.

```text
$ git add .
$ git commit -m "a message explaining your modification"
$ git push -u origin master
```

{% hint style="info" %}


* List of [commonly used gitignore files](https://github.com/github/gitignore)
{% endhint %}

