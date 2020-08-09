# Git Setup and Basics

**REVIEW THIS AND COMBINE WITH GIT AND GITHUB MATERIALS IN THE TEMPLATE**

## Getting setup with Git and GitHub

We will use Git and Github for collaborative work. Be sure to arrive at OceanHackWeek with your own [GitHub](https://github.com/) account.

## Git Installation

- Windows
    - You need to install Git for Windows from this [link](https://gitforwindows.org/). For more setup details follow these [instructions](https://carpentries.github.io/workshop-template/#shell)
- MAC OS
    - Download the [git installer](https://git-scm.com/download/mac) and run it.
- Linux (Debian)
    ```
      sudo apt install git-all
    ```
    
To test open the terminal (on Windows, Git Bash) and setup your username and email:

```
  git config --global user.name "your username"
  git config --global user.email "your email"
```
 

## Getting started with Bash

During the hackweek it will be useful to know how to navigate between files from the command line. If you are not familiar with the unix shell commands you can review the first three sections of this [Software Carpentry Shell Novice](https://swcarpentry.github.io/shell-novice/) lesson. On Windows, use the Git Bash terminal to run these commands.


## Command line editor

When working on the command line, it is often handy to modify file content directly from there. For that you can use a command line editor such as `nano`. On Mac and Linux it is usually pre-installed, but for Windows you can follow the instructions in this [link](http://carpentries.github.io/workshop-template/#editor) to set it up. Test your installation by opening a terminal and running `nano --version`. If it works you can link your github with nano:

```
git config --global core.editor "nano -w"
```

## Resources

Git and GitHub are very powerful tools but no doubt the learning curve is steep. Although we will cover some of the basics at Oceanhackweek, learning is an iterative process so below we list some resources which can help you be better prepared:

[What is GitHub?](https://www.youtube.com/watch?v=w3jLJU7DT5E) (3:45 min)

[CUAHSI Tutorial](https://www.youtube.com/watch?v=Bc5BO9gPC9w&feature=youtu.be) (1 hour)

[Software Carpentry Lesson](http://swcarpentry.github.io/git-novice/) (3 hours with exercises)

[GitHub Learning Lab](https://lab.github.com/): practice with a bot! (On your own pace)