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

### Making Changes

Now that you are working on your own branch, you can make changes to the files in the repository. For this exercise, you will add your name to the list of champions in the `champions.md` file. Open the `champions.md` file in your text editor, and add your name or username to the list, prefixed with an asterisk (`*`). For example, if your username is `brendonthiede`, you would add the following line to the file:

```text
* brendonthiede
```

Once you have added your name, save the file. Now when you run `git status`, you should see something like the following:

```text
On branch adding-brendonthiede
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   champions.md

no changes added to commit (use "git add" and/or "git commit -a")
```

### Committing Changes

Once you have made changes to the files in the repository, you can commit those changes to your local copy of the repository. This allows you to keep track of the changes you make to the repository over time. To commit your changes, run the following command in the terminal:

```bash
git add champions.md
git commit -m "Adding brendonthiede to champions list"
```

The first command stages the changes you made to the `champions.md` file, and the second command commits those changes to your local copy of the repository with the message provided. You can now run `git status` again, and you should see something like the following:

```text
On branch adding-brendonthiede
nothing to commit, working tree clean
```

### Pushing Changes

Once you have committed your changes to your local copy of the repository, you can push those changes to the remote copy of the repository on GitHub. To push your changes, run the following command in the terminal:

```bash
git push origin adding-brendonthiede
```

"origin" is the name for the GitHub "remote" that was added automatically when we first cloned the repo from there. "adding-brendonthiede" is the name of the branch that we are pushing to the remote. You should now see your changes on GitHub, in your forked copy of the repository.

### Creating a Pull Request

Now that you have pushed your changes to your forked copy of the repository, you can create a pull request to merge your changes into the original repository. To create a pull request, go to your forked copy of the repository on GitHub, and click the "Pull requests" tab. Then click the "New pull request" button. This will open a page where you can review the changes you are requesting to merge into the original repository. If everything looks good, click the Create pull request button. This will open a page where you can add a title and description for your pull request. Once you have added a title and description, click the "Create pull request" button. This will create a pull request, and open a page where you can see the status of your pull request. Once your pull request has been reviewed and merged, you will see your changes in the original repository.
