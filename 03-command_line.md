# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > 1. pwd: show current working directory path
2. mkdir: create directory
3. rm -r: delete directory
4. touch: create file
5. rm: remove file
6. mv: rename file [mv fileName newName]
7. ls -a: list hidden files
8. cp: copy file from one diretory to another [cp argument target]
9. grep: search files for line matching pattern and returns results, case sensitive
10. cd: change directory

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > ls: lists all files in the directory
ls -a: lists all files including hidden ones
ls -l: lists files in long format
ls -lh: lists long format, readable size
ls -lah: lists long format, readable size,  including hidden files
la -t: sort by time and date
ls -Glp: list in long format without group names and append / indicator to directories
---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > 1. -d: displays only directories
2. -r: displays files in reverse order
3. -R displays recursively directory tree
4. -1: displays each entry on a line
5. -m: displays names as a comma separated listt

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> >Used in combination with command line commands, xargs converts standard input into arguments to a command and then executes the commands for each arguments.
For example, if I wanted to search for files in a directory and remove the results, I could use xargs in the following way:
	find /path -name "someFileType" | xargs rm

 

