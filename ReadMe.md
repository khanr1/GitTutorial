# Introduction

This project is my notes about the basic commands of git hubs. All the command line are made in a Linux environment and how to start a project. Some references for this notes are

1. [openclassrooms](https://openclassrooms.com/courses/gerer-son-code-avec-git-et-github)
2. [Try git: git tutorial](https://try.github.io/levels/1/challenges/1)

# Starting a new project

In general, the first thing to when starting a new project (independently of git hub) is to create a folder where the root of the project will be for the purpose of these notes I created a folder named GitTutorial. To initialize the git repository we go in the folder that we just created and type `git init`

```bash
mkdir GitTutorialit
cd GitTutorial
git init
```
the last command initialize a git repository. with the command `git status` you can
see the current state of the project. Since we have done nothing at the moment, it
should return:
```bash

On branch master

Initial commit

nothing to commit (create/copy files and use "git add" to track)
```
We have nothing here, however we are in a git repository which is where and what we  want to start our new project.

# First commit

Now that we have created our git repository, lets add a ReadMe.md file which describe
the project (In fact the ReadMe will contains all my notes on git). We create this new file  using the command `touch ReadMe.md` (or any prefered way). Checking the state
of the project will now give us

```bash
git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	ReadMe.md

nothing added to commit but untracked files present (use "git add" to track)
nothing to commit (create/copy files and use "git add" to track)
```
We see that ReadMe.md is not track by git. For changing that one need to add the file to the git index with the following command
```bash
git add ReadMe.md
```
The file is now added to the git index and git will keep track of any changes in the file. Looking at the status of the project one get that there are changes needed
to  be committed i.e. which need to be looged and saved in the local repository. This is done with to following command
```bash
git commit -m "First commit"
[master (root-commit) 14bee8e] First commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 ReadMe.md
```


git remote add origin https://github.com/khanr1/GitTutorial.git
git push -u origin master
