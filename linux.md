# Linux

- [Overview](#Overview)
- [Commands](#Commands)
- [Flags](#Flags)
- [Linux Directory Structure](#Linux-Directory-Structure)

---

## Overview

***The GNU Project**, started in 1983 by Richard Stallman, had the goal of creating a "complete Unix-compatible software system" composed entirely of free software. Work began in 1984. Later, in 1985, Stallman started the Free Software Foundation and wrote the GNU General Public License (GNU GPL) in 1989. In 1991, while attending the University of Helsinki, Linus Torvalds became curious about operating systems. Frustrated by the licensing of MINIX, which at the time limited it to educational use only, he began to work on his own operating system kernel, which eventually became the **Linux kernel**. Thus **GNU Linux**, an open source UNIX operating system based on **Linux kernel** created in 1991 by Linus Torvalds was born after combining with Richard Stallman's GNU license.

Features of linux are:*
- *Linux is portable i.e, linux kernel and application programs supports their installation on any kind of hardware platform.*
- *Being open-source, anyone with programming knowledge can modify it.*
- *The freedom to distribute copies of your modified versions to others.*
- *Linux is a multiuser system means multiple users can access system resources like memory/ ram/ application programs at same time.*
- *Linux is the OS of choice for Server environments due to its stability and reliability (Mega-companies like Amazon, Facebook, and Google use Linux for their Servers). A Linux based server could run non-stop without a reboot for years on end.*

*Linux is also distributed under an open source license. Some of the most popular Linux based distributions or distros are: 
- *Ubuntu*
- *Fedora*
- *Mint*
- *Debian*

## Linux Architecture
![Linux Architecture](https://github.com/Dipankar-Chakraborty/missingskill-learning/blob/main/images/linux-architecture.jpg)
---

## Commands

 **Directory Commands**
  - *__pwd__ - path of the present working directory. Example: __/home/dipankar__*
  - *__cd__ - change directory. Example: __cd..__(with two dots) to move one directory up, __cd__ to go straight to the home folder, __cd__-(with a hyphen) to move to previous directory*
  - *__ls__ - show the list of files and folders present in the directory. Example __```ls /home/dipankar/documents```__*
  - *__mkdir__ - make a new directory. Example: __```mkdir movie```__ would create a new directory movie*
  - *__rmdir__ - removes empty directories. Example: __```rmdir mydir```__ removes mydir if it's empty, __```rmdir dir1 dir2 dir3```__ removes the directories dir1, dir2, and dir3, if they are empty. Else, an error message will be printed for non-empty directory and the others will be removed*
 
   **File Commands**
  - *__touch__ - create a new file. Example: __```touch /home/dipankar/documents/bills.txt```__ will create a txt file under the Documents directory*
  - *__rm__ - remove a file*
  - *__cp__ - copy files from the current directory to a different directory. Example: __```cp bills.pdf /home/dipankar/documents```__ would create a copy of bills.pdf (from current directory) into the documents directory.*
  - *__mv__ - move and rename a file. Example: __```mv bills.pdf /home/dipankar/documents```__ will move bills.pdf to documents*
  - *__rename__ - rename a file*
  - *__cat__ - create, display contents and concatenate files. Example: __```cat>filename```__ creates a new file, __```cat f1 f2>f3```__ joins files f1 and f2 and stores their output in f3*
  - *__echo__ - move some data into a file. Example, __```echo Hello, my name is Dipankar >> name.txt```__ will add the text into a file called name.txt*
  - *__head__ - view the first lines of any text file.Example: __```head -n 5 docs.txt```__ will show the first five lines of the docs.txt file*
  - *__tail__ - view the last 10 lines of any text file.Example: __```tail -n docs.txt```__ will show the last ten lines of the docs.txt file*
  - *__which__ - locate executable files*
  - *__whoami__ - show system's username*
  - *__who__ - show logged users*
  - *__ping__ - check connectivity with internet.Example ```ping google.com```*
  - *__wget__ - download files from a server*
  
  ## Flags
    **ls -l-h-t-r-F**
   - *__ls__ - list all files in details*
   - *__l__ - list*
   - *__h__ - human readable*
   - *__t__ - latest file at top*
   - *__r__ - old file at top*
   - *__F__ - adds slash at the end* 
  
  ## Linux Directory Structure
  ![Linux Directory Structure](https://github.com/Dipankar-Chakraborty/missingskill-learning/blob/main/images/linux-directory-structure.jpg)
 ---
