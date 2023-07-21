# Git & Github Tutorial for Noobies :tada:

Welcome to the Git & Github tutorial! In this guide, we'll cover the basics of using Git and Github for version control and collaborative development. Git is a distributed version control system that helps developers track changes to their code over time, while Github is a web-based hosting service for Git repositories, enabling collaboration and sharing of code. :octocat:

## Table of Contents 
1. [Getting Started](#1-getting-started)
2. [Staging and Committing Changes](#2-staging-and-committing-changes)
3. [Using Git with VS Code](#3-using-git-with-vs-code)
4. [Working with Remote Repositories](#4-working-with-remote-repositories)
5. [Pushing Changes to a Remote Repository](#5-pushing-changes-to-a-remote-repository)
6. [Merging Branches](#6-merging-branches)
7. [Pulling Changes from Remote](#7-pulling-changes-from-remote)
8. [Cloning a Repository](#8-cloning-a-repository)
9. [Working with Branches](#9-working-with-branches)
10. [Handling Merge Conflicts](#10-handling-merge-conflicts)
11. [Forking a Repository](#11-forking-a-repository)
12. [Making Pull Requests](#12-making-pull-requests)
13. [Git Reset](#13-git-reset)
14. [Git Revert](#14-git-revert)
15. [Git Amend](#15-git-amend)
16. [Git Stash](#16-git-stash)
17. [Git Rebase](#17-git-rebase)
18. [Git Squash](#18-git-squash)

## 1. Getting Started 

Let's begin by initializing a Git repository in your project folder:

```bash
git init
```

## 2. Staging and Committing Changes

Once you've made some changes to your project, you can stage them for commit using the following command:

```bash
git add .
```
The above command stages all the changes in your project for the next commit. However, if you want to unstage some changes, you can use:

```bash
git reset . 
```

You can check the status of your repository and see which files are staged or unstaged using:

```bash
git status
```

Once you have staged the changes, you can commit them with a meaningful message:
```bash
git commit -m "Your commit message here"

```

You can view the commit history using:

```bash
git log
```

For a more condensed and graphical representation, you can use:

```bash
git log --graph --oneline --decorate
```

## 3. Using Git with VS Code
If you're using Visual Studio Code as your code editor, you can take advantage of Git integration using extensions like "Git Lens" and "Git Source Control."

## 4. Working with Remote Repositories
To connect your local repository to a remote repository (like one hosted on Github), use the following command:

```bash
git remote add origin <git url>

```
## 5. Pushing Changes to a Remote Repository
To push your changes to the remote repository (specifically to the "master" branch), use:

```bash
git push origin master -u

```
The -u flag sets the "origin" as the default upstream remote, simplifying future pushes.



## 6. Merging Branches
You can merge changes from one branch into another using various merge strategies. For example, to perform a Fast-Forward merge (when there are no conflicting changes):

```bash
git fetch
git merge origin/master
```



7. Pulling Changes from Remote
To pull changes from the remote repository (fetch + merge):

```bash
git pull

```
Remember to stash or commit local changes before pulling, as it may cause merge conflicts.



## 8. Cloning a Repository
To clone an existing repository from a remote source, use:

```bash
git clone <repository url>

```

## 9. Working with Branches
You can list all branches in your repository using:

```bash
git branch
```
To create a new branch and switch to it:

```bash
git checkout -b new-branch
```
To delete a branch:

```bash
git branch -d branch-name
```
Use -D instead of -d if you want to forcefully delete a branch.



## 10. Handling Merge Conflicts
Merge conflicts occur when Git can't automatically merge changes. You'll need to manually resolve conflicts and then commit the changes.


## 11. Forking a Repository
Forking allows you to create your own copy of a repository on your Github account, enabling you to make changes without affecting the original repository.

## 12. Making Pull Requests
To contribute to a project, you can follow these steps:

Fork the repository on Github.
Clone the forked repository to your local machine.
Create a new branch for your feature/fix.
Commit and push your changes to your fork.
Create a pull request on Github to propose your changes to the original repository.

when working with fork locally we can keep it in sync with the original


```bash
git remote add upstream < git url>
git fetch upstream
git rebase upstream/master
```
 

## 13. Git reset

Git reset allows you to unstage changes from the staging area.

```bash
git reset
```
You can also reset to a specific commit by using the commit ID:

```bash
git reset <commit-id>

```

## 14. Git Revert
Git revert is used to undo a previous commit by creating a new commit with the opposite changes.

15. Git Amend
Git amend is used to modify the last commit.

```bash
git commit --amend "Your updated commit message"

```

```bash
git commit --amend --no-edit # (forgot to add some files to staging before the commit )

```



## 16. Git Stash
Git stash allows you to temporarily store changes that are not ready to be committed.

```bash
git stash save "Your stash message"


```
To apply the changes back:
```bash
git stash apply

```





## 17. Git Rebase
Git rebase is used to modify the commit history by moving, combining, or deleting commits.

 
## 18. Git Squash
Git squash is used to combine multiple commits into one.

```bash
git rebase -i master
```

Replace "pick" with "squash" for the commits you want to squash.

Feel free to use this tutorial as a starting point and add more details, examples, and styling as needed. Happy coding with Git and Github!
