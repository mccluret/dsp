# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy`s Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here`s a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > 1) `pwd` - Shows current working directory path.
> > 2) `mkdir dir-name` - Makes a new directory.
> > 3) `rm -r dir-name` - Removes a directory. 
> > 4) `touch file1 file 2 file3` - Makes new file(s).
> > 5) `rm file-name` or `rm -f _file-name_` - Deletes file, and deletes file forecfully without prompting.
> > 6) `mv file-name_ _file-newName_` - Renames by moving the file to the same location under a new name.
> > 7) `ls -a` - Lists files in current directory, including hidden files. 
> > 8) `cp file-name new-directory` - copies file into new directory.
> > 9) `echo "This text is appended to a new file" >> newFile.txt` - Added text to the end of a file, a new one.
> > 10) `cd ..` - Moves up a directory.
> > 11) `date` - Shows system date
> > 12) `git init` - Creates files fro version control
> > 13) `git add -A` - Adds all changes to the next commit, including removals.
> > 14) `git branch -r` - List all remote branches.
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

> > 1) `ls` - Lists files and directories.
> > 2) `ls -a` - lists all including hidden. 
> > 3) `ls -l` - long format, displaying file types, permissions, number of hard links, etc.
> > 4) `ls -lh` - long format with print sizes in human readable format. ex 4.5k vs 4500
> > 5) `ls -lah` - long format, including hidden files, with sizes in readable format.  
> > 6) `ls -t`  - sort the list by modification time.
> > 7) `ls -Glp` - G: freeBSD checks unix file, permissions and uses the termcap db. lp: long and adds / to dirs

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > 1) `ls -l --color` - long list and color coordinates different files.
> > 2) `ls -f` - do not sort, good for directories with large numbers of files.
> > 3) `ls -R` - lists subdirectories with directories.
> > 4) `ls -F` - appends a character for file typesuch as * for exe and / for dir.
> > 5) `ls -1` - displays each entry on a line.

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > Xargs takes standard input (stdin) and executes the command (supplied to it as an argument). Default is echo.  
> > This means it can be used to print, prompt, read inputs from a file. etc.  
> > **Example:** `find . -name '*.py' | xargs wc -l` - This recursively finds all python files and count the number of lines.   
> > **Example:** `find . -name '*~' -print0 | xargs -0 rm` - handling spaces; removes backup files recursively even with spaces.  
 

