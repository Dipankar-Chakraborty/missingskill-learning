# Linux

- [Overview](#Overview)
- [Commands](#Commands)

---

## Overview

Linux is an open source UNIX operating system created in 1991 by Linus Torvalds. Features of linux are:
- Linux is portable i.e, linux kernel and application programs supports their installation on any kind of hardware platform.
- Being open-source, anyone with programming knowledge can modify it.
- The freedom to distribute copies of your modified versions to others.
- Linux is a multiuser system means multiple users can access system resources like memory/ ram/ application programs at same time.
- Linux is the OS of choice for Server environments due to its stability and reliability (Mega-companies like Amazon, Facebook, and Google use Linux for their Servers). A Linux based server could run non-stop without a reboot for years on end.

Linux is also distributed under an open source license. Some of the most popular Linux based distributions or distros are: 
- Ubuntu
- Fedora
- Mint
- Debian

---

## Commands

 **Directory Commands**
  - *__pwd__ - path of the present working directory. Example: __/home/dipankar__*
  - *__cd__ - change directory. Example: __cd..__(with two dots) to move one directory up, __cd__ to go straight to the home folder, __cd__-(with a hyphen) to move to previous directory*
  - *__ls__ - show the list of files and folders present in the directory. Example __ls /home/dipankar/documents__*
  - *__mkdir__ - make a new directory. Example: __mkdir movie__ would create a new directory movie*
  - *__rmdir__ - removes empty directories. Example: __rmdir mydir__ removes mydir if it's empty, __rmdir dir1 dir2 dir3__ removes the directories dir1, dir2, and dir3, if they are empty. Else, an error message will be printed for non-empty directory and the others will be removed*
 
   **File Commands**
  - *__touch__ - create a new file. Example: __touch /home/dipankar/documents/bills.txt__ will create a txt file under the Documents directory*
  - *__rm__ - remove a file*
  - *__cp__ - copy files from the current directory to a different directory. Example: __cp bills.pdf /home/dipankar/documents__ would create a copy of bills.pdf (from current directory) into the documents directory.*
  - *__mv__ - move and rename a file. Example: __mv bills.pdf /home/dipankar/documents__ will move bills.pdf to documents*
  - *__rename__ - rename a file*
  - *__cat__ - create, display contents and concatenate files. Example: __cat>filename__ creates a new file, __cat f1 f2>f3__ joins files f1 and f2 and stores their output in f3*
  - *__echo__ - move some data into a file. Example, __echo Hello, my name is Dipankar >> name.txt__ will add the text into a file called name.txt*
  - *__head__ - view the first lines of any text file.Example: __head -n 5 docs.txt__ will show the first five lines of the docs.txt file*
  - *__tail__ - view the last 10 lines of any text file.Example: __tail -n docs.txt__ will show the last ten lines of the docs.txt file*
  - *__which__ - locate executable files*
  - *__whoami__ - show system's username*
  - *__who__ - show logged users*
  - *__ping__ - check connectivity with internet*
  - *__wget__ - download files from a server*
  
 ---
