<img src="https://fullstackbd.com/assets/images/logo-with-name.png" width="80" />

# Git And Github

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
  - [Windows](#windows)
  - [Mac](#mac)
  - [Linux](#linux)
- [Creating a Local Folder and Linking it to GitHub](#creating-a-local-folder-and-linking-it-to-github)
- [Creating a Git Repository and cloning it](#creating-a-git-repository-and-cloning-it)

## Introduction

Git is a distributed version control system that allows you to track changes to your code over time. It was created by Linus Torvalds in 2005 to help manage the development of the Linux kernel. With Git, you can create a repository to store your code and collaborate with others by sharing your changes and merging them with others' changes.

## Installation

### Windows

1. Download the latest Git for Windows installer.
2. When you've successfully started the installer, you should see the Git Setup wizard screen. Follow the Next and Finish prompts to complete the installation. The default options are pretty sensible for most users.

### Mac

1. Download the latest Git for Mac installer.
2. Follow the prompts to install Git.
3. Open a terminal and verify the installation was successful by typing git --version:

### Linux

1. You can install Git in a number of ways, depending on your Linux distribution. If you're on Fedora (or any closely-related RPM-based distribution, such as RHEL or CentOS), you can use dnf:

```
$ sudo dnf install git-all
```

2. If you're on a Debian-based distribution, such as Ubuntu, try apt:

```
$ sudo apt install git-all
```

## Creating a Local Folder and Linking it to GitHub

1. **Create a new repository on GitHub.**

- Navigate to [GitHub](https://github.com/).
- Click on the '+' button on the upper right corner and select 'New repository'.
- Name your repository and provide a description (optional).
- Choose to make the repository either public or private.
- Click 'Create repository'.

2. **Create a new directory on your local machine.**

- Open a terminal.
- Navigate to the location where you want to create the directory using `cd` command.
- Create a new directory using `mkdir your-directory-name`.

3. **Initialize the local directory as a Git repository.**

- Navigate into the new directory using `cd your-directory-name`.
- Initialize the directory as a Git repository using `git init`.

4. **Create and Add Files.**

- Create a new file.
- Add the file to the staging area using `git add .`.
- Commit the file using `git commit -m 'First commit'`.
- Set the branch to main using `git branch -M main`.

4. **Link the local repository to the GitHub repository.**

- Use the command `git remote add origin your-github-repository-url`.

6. **Push local changes to the GitHub repository.**

- Push the changes in your local repository to GitHub using `git push -u origin main`.

## Creating a Git Repository and cloning it

1. **Create a new repository on GitHub.**

- Navigate to [GitHub](https://github.com/).
- Click on the '+' button on the upper right corner and select 'New repository'.
- Name your repository and provide a description (optional).
- Choose to make the repository either public or private.
- Click 'Create repository'.

2. **Clone the repository.**

- Open a terminal.
- Navigate to the location where you want to clone the repository using `cd` command.
- Clone the repository using `git clone your-github-repository-url`.
