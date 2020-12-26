# introduction

### Why Git

#### How to Install Git

There are several ways to install Git for your computer \([https://git-scm.com/book/en/v2/Getting-Started-Installing-Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)\). If you have installed Anaconda, you can simply run the following command in your terminal

```text
$ conda install git
```

#### How to use Git

There are several graphical interface to use git, however I recommend my students to use classical git command from terminal. A wonderful ressource to learn git is the Pro Git book written by Scott Chacon and Ben Straub and published by Apress.

* [Pro Git Book](https://github.com/progit/progit2/releases/download/2.1.277/progit.pdf)

All the power of git relies on the use of several web plateform for code sharing, reviewing and more. There are basically two options :

* [Github](https://github.com) :  The Github plateform allows you to share, distribute your code for free \(there are also non-free plan for more specific usage\). 
* [Gitlab](https://about.gitlab.com/install/) : Gitlab is also quite popular in many tech firms. As compared to Github, Gitlab can be installed on your private server. There is a very high probability that your school or institution has a fully functionnaly git server.

### Command Snippests

```text
$ git add .
$ git commit -m "my first commit"
$ git push -u origin master
```

{% hint style="info" %}
For your projects, I recomment to use a `.gitignore` file to avoid to keep track of non essential files. The content of this file depends on the nature of your project.

* List of [commonly used gitignore files](https://github.com/github/gitignore)
{% endhint %}







