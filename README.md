# lhh-github-intro

An introduction to using GitHub

## Description

This is a Git repository hosted on GitHub. By following this tutorial, you will learn how to use Git and GitHub to collaborate on a project with other people, while keeping track of the changes you make to your files. In order to follow all of the steps here, you will need a computer with some software installed, as well as a GitHub account. If you don't have a GitHub account, you can create one for free at [github.com](github.com).

## Getting Started

### Installing Git

Git is a version control system that allows you to keep track of changes you make to your files. It is also a distributed version control system, which means that you can work on your files locally, and then push your changes to a remote repository, such as one hosted on GitHub. In order to use Git, you will need to install it on your computer. If you are using a Mac, you can install Git by following the instructions at [git-scm.com/download/mac](https://git-scm.com/download/mac). If you are using Windows, you can install Git by following the instructions at [git-scm.com/download/win](https://git-scm.com/download/win). Many Linux distributions come with Git already installed, but if you need to install it, you can follow the instructions at [git-scm.com/download/linux](https://git-scm.com/download/linux).

### Installing VS Code

VS Code is an Integrated Development Environment, commonly called an IDE, that you can use to write code and edit files. VS Code also has built in source control features that can make it easier to use Git. VS Code is free and open source, and it is available for Windows, Mac, and Linux. You can download VS Code at [code.visualstudio.com](https://code.visualstudio.com/). If you don't want to use VS Code, you can use any text editor you like, such as Notepad, TextEdit, or Sublime Text.

### Forking this Repository

Specifically for GitHub, it is a common practice to begin working on a project by forking the repository. Forking a repository creates a copy of the repository in your own GitHub account. To fork this repository, click the Fork button in the upper right corner of this page. This will create a copy of this repository in your own GitHub account.

### Cloning the Repository

Once you have forked this repository, you will need to clone it to your computer. Cloning a repository creates a copy of the repository on your computer. To clone this repository, click the green Code button in the upper right corner of this page (when viewing from your forked repository's page). This will open a menu that will allow you to copy the URL of the repository. There are multiple options for connection to the repo, but I recommend using HTTPS as the option for now, as it is the easiest to get going with, and it is quite secure. Copy the URL of the repository, and then open a terminal on your computer. In the terminal, navigate to the directory where you want to clone the repository. You should use a directory that will be used specifically for code, so that it doesn't get lost with other files. One example would be to create a directory named `code` in your home directory, and then clone the repository there. Once you have navigated to the directory where you want to clone the repository, run the following command, replacing the URL with the URL of your forked repository:

```bash
git clone https://github.com/your_github_username/lhh-github-intro.git
```

You should now see a new directory named `lhh-github-intro` in the directory where you cloned the repository. This directory contains all of the files in the repository. You can now open this directory in VS Code, or your preferred text editor. For VS Code, you can open the directory by running the following command in the terminal:

```bash
code lhh-github-intro
```

### Checking the Status of the Repository

Once you have cloned the repository, you can check the status of the repository by running the following command in the terminal from inside the directory where you cloned the repository:

```bash
git status
```

This will show you the current status of the repository. You should see something like the following:

```text
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```

### Creating a Branch

When working on a project, it is common to create a new branch before you start working on new things, often called "features". This allows you to work on multiple features at the same time, without having to worry about changes to one feature affecting another feature. For this exercise you will create a branch named `adding-<username>`, where you replace `<username>` with your GitHub username. To create a new branch for the user `brendonthiede`, run the following command in the terminal:

```bash
git checkout -b adding-brendonthiede
```

Now when you run `git status`, you should see something like the following:

```text
On branch adding-brendonthiede
nothing to commit, working tree clean
```
