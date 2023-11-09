<img src="https://fullstackbd.com/assets/images/logo-with-name.png" width="150" />

# Git And Github

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
  - [Windows](#windows)
  - [Mac](#mac)
  - [Linux](#linux)
- [Creating a Local Folder and Linking it to GitHub](#creating-a-local-folder-and-linking-it-to-github)
- [Creating a Git Repository and cloning it](#creating-a-git-repository-and-cloning-it)
- [Branching](#branching)
- [Pull Requests](#pull-requests)
- [Forking](#forking)
- [Branch Strategy](#branch-strategy)
- [Collaborating](#collaborating)

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

## Adding Files

1. **Add a single file.**

- Add a file to the staging area using `git add your-file-name`.

2. **Add multiple files.**

- Add all files to the staging area using `git add file1 file2`.

3. **Add all files.**

- Add all files to the staging area using `git add --all`.

4. **Add files from a specific directory.**

- Add all files from a specific directory to the staging area using `git add .` or `git add directory-name`.

## Committing Files
```bash
$ git commit -m 'Commit message'
```

## Pushing Files

1. **Push files to the main branch.**

- Push files to the main branch using `git push origin main`.

2. **Push files to a specific branch.**

- Checkout to the specific branch using `git checkout your-branch-name`.
- Push files to a specific branch using `git push origin your-branch-name`.

## Pulling Files

1. **Pull files from the main branch.**

- Pull files from the main branch using `git pull origin main`.

2. **Pull files from a specific branch.**

- Pull files from a specific branch using `git pull origin your-branch-name`.

## Branching

1. **Create a new branch.**

- Open a terminal.
- Navigate to the location of the repository using `cd` command.
- Create a new branch using `git branch your-branch-name`.

2. **Switch to the new branch.**

- Switch to the new branch using `git checkout your-branch-name`.

3. **Push the new branch to the remote repository.**

- Push the new branch to the remote repository using `git push origin your-branch-name`.

4. **Merge the new branch with the main branch.**

- Switch to the main branch using `git checkout main`.
- Merge the new branch with the main branch using `git merge your-branch-name`.

5. **Delete the new branch.**

- Delete the new branch using `git branch -d your-branch-name`.

## Pull Requests

1. **Why do we need pull requests?**

- Pull requests are a way to propose changes to a repository. They notify project maintainers about the changes you want to make in your repository. Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before the changes are merged into the repository.

2. **How to create a pull request?**

- Navigate to the repository on GitHub.
- Click on the 'Pull requests' tab.
- Click on the 'New pull request' button.
- Select the branch you want to merge into the main branch.
- Click on the 'Create pull request' button.
- Add a title and description to your pull request.
- Click on the 'Create pull request' button.

3. **How to merge a pull request?**

- Navigate to the repository on GitHub.
- Click on the 'Pull requests' tab.
- Click on the pull request you want to merge.
- Click on the 'Merge pull request' button.
- Click on the 'Confirm merge' button.

## Forking

1. **Why do we need forking?**

- Forking a repository allows you to freely experiment with changes without affecting the original project. Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea.

2. **How to fork a repository?**

- Navigate to the repository on GitHub.
- Click on the 'Fork' button on the upper right corner.

3. **How to create a pull request from a forked repository?**

- Navigate to the forked repository on GitHub.
- Click on the 'Pull requests' tab.
- Click on the 'New pull request' button.
- Select the branch you want to merge into the main branch.
- Click on the 'Create pull request' button.
- Add a title and description to your pull request.
- Click on the 'Create pull request' button.

4. **How to merge a pull request from a forked repository?**

- Navigate to the forked repository on GitHub.
- Click on the 'Pull requests' tab.
- Click on the pull request you want to merge.
- Click on the 'Merge pull request' button.
- Click on the 'Confirm merge' button.

## Branch Strategy

1. **Why do we need a branch strategy?**

- A branch strategy is a set of rules that a team agrees to follow when using branches. It helps to keep the repository organized and makes it easier to manage changes.

2. **What are the different types of branches?**

<img src="https://i.imgur.com/aHBHpVn_d.webp?maxwidth=760&fidelity=grand" />

- Main branch: The main branch is the default branch when you create a repository. It is also known as the master branch. It should always contain the latest stable version of the code.
- Development branch: A development branch is used to develop new features. It is created from the main branch and merged back into the main branch when the feature is complete.
- Feature branch: A feature branch is used to develop a new feature. It is created from the main branch and merged back into the main branch when the feature is complete.
- Release branch: A release branch is used to prepare a new release. It is created from the main branch and merged back into the main branch when the release is ready.
- Hotfix branch: A hotfix branch is used to fix a bug in the code. It is created from the main branch and merged back into the main branch when the bug is fixed.

<!-- provide a image of the branch strategy -->

## Collaborating

1. **How to add collaborators to a repository?**

- Navigate to the repository on GitHub.
- Click on the 'Settings' tab.
- Click on the 'Manage access' button.
- Click on the 'Invite a collaborator' button.
- Enter the username or email address of the collaborator.
- Click on the 'Add username/email' button.

2. **How to accept a collaboration invitation?**

- Navigate to Github.
- Click on the 'Invitations' tab.
- Click on the 'Accept invitation' button.

3. **How to remove a collaborator from a repository?**

- Navigate to the repository on GitHub.
- Click on the 'Settings' tab.
- Click on the 'Manage access' button.
- Click on the 'Remove' button next to the collaborator you want to remove.
