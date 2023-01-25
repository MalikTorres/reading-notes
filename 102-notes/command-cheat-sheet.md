# Command Line Cheat Sheet

* `-` dash represents and option and are typycally listed before arguements

* _shell refers to the inside of the terminal_
    * Common shell is **bash**
    * **echo** displays current shell

* refer to previous commands by using the up and down arrows 

* **file** can be used to determine which type of file something is 

_Specification of a file is a path(file location)_

_Files need to be seen as single line arguements within the terminal_ 
   * Quotes `""` can be used to create single line arguements (single or double)
   * Backslash `/` can be used as well, as they are an escape character and nulify the meaning of the next character 

* Hidden files can refer to files such as configurition files which are hidden so they do not interfere with the users daily task 

* `a .` can be used to hide files

* `ls -a` list content including hidden files 

* `pwd` print working directory

*`[]` the items shown in the terminal are optional 

* `-l` indiciates long listing 

* `path` how to access a certain file or directory
    *  **absolute** and **relative** 

* root directory is noted by a single `/` 

* abosolute paths begin with `/`

* relative paths do not being with `/` 
    * relative paths specify paths in relation to where they are located in the system 

* `~` shortcut for home directory

* `.` reference to current directory 

* `..` can be used to access parent directory 

* `cd` change directory 

* `ls` list contents of a directory

* use tab to auto complete 

* `git config` allows the setting of configuration variables

* `git config --global user.name` to verify correct name

* `git config --global user.email` to verify correct email

* `-global` settings apply to anything ont he system

* `git config --list` to check settings 

* `git help` command for help

* `git` command `--help`

**Importing** 

* Switch to the target projects's directory `cd`

* Use the git init command `git init` 

**Tracking not commenced after creating subdirectory named .git** 

_To track perform `git add` and `git commit` 

`git clone` to copy an existing Git repository from a particular server by using the `git clone` command and URL

**Local Repository structure**

* Working directory: Where files are

* Index: Stage area

* Head: Points to the most recent commit 

* `git stash` to remove unwanted commits 

* `git stash apply` to retrive stashed commands

**Things I would like to know more about** 

* Git commands to edit specific commits

* In general commands to make edits within my terminal after mistyping a command



