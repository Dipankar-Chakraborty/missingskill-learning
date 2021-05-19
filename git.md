# Git

- [Overview](#Overview)
- [Commands](#Commands)

---

## Overview

*__Linus Torvalds__, the developer of the Linux kernel, created Git in __2005__ to help control the Linux kernel's development. Git is an __open-source distributed version control system__ that developers use to __collaborate__ on projects of any scale for __developing software and applications__. Git allows to __track changes__ made to files. Git is a distributed version control system, meaning __local copy of code is a complete version control repository__. These fully-functional local repositories make it is easy to __work offline or remotely__. We can __commit our work locally, and then sync our copy of the repository with the copy on the server__.*

*A Git project consists of three major sections: __the working directory, the staging area, and the git directory__.*

*The working directory is where we __add, delete, and edit the files__. Then, the changes are __staged (indexed)__ in the staging area. After we __commit our changes__, the snapshot of the changes will be saved into the git directory.*

*Git's goals include __speed, data integrity, and support for distributed, non-linear workflows__. Everyone can use Git as it is available for __Linux, Windows, Mac, and Solaris.__*

---

## Commands

  - *__git config__ - sets user-specific configuration values like email, username.*  
  ```git config --global user.name "Dipankar"```
  - *__git init__ - creates a new empty repository.*  
  ```git init```
  - *__git clone__ - creates a copy of repository.*   
  ```git clone https://github.com/Dipankar-Chakraborty/missingskill-learning.git```
  - *__git add__ - adds one or more files to the staging area.*  
  ```git add hello.txt```
  - *__git commit__ - creates a snapshot of the changes and saves it to the git directory.*  
  ```git commit -m "Updated git.md"```
  - *__git status__ - displays the state of working directory i.e, list of changed files together with the files that are yet to be staged or committed.*
  ```git status```
  - *__git push__ - uploads contents of local repository to remote repository after commit.*   
  ```git push origin branch1```
  - *__git pull__ - merges all the changes present in the remote repository to the local working directory.*   
  ```git pull```
  - *__git branch__ - list, create, or delete branches.*  
  ```git branch```
  - *__git merge__ - merges a branch into the present branch.*  
  ```git merge branch2```
  - *__git log__ - to see the repository’s history by listing certain commit’s details.*  
  ```git log```
  - *__git diff__ - lists down changes made in the working directory and index.*  
  ```git diff branch1 branch2```
  - *__git checkout__ - to navigate between branches and switch to a different branch.*  
  ```git checkout branch1```
  - *__git reset__ - reset the index and the working directory to the git's last commit state.*  
  ```git reset```
  - *__git stash__ - temporarily saves the changes that are not ready to be committed.*  
  ```git stash```
  - *__git remote__ - lists all remote repositories.*  
  ```git remote```
  - *__git fetch__ - fetches all objects from the remote repository that don’t currently reside in the local working directory.*  
  ```git fetch origin```

---
