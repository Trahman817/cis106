 
 ## Question 1
 ## ls

# Definition:
ls lists files and directories in a folder.

# Usage:
By default, ls lists the contents of the current directory. You can also specify a directory or file to list.
# Formula
 bash 
 ls [options] [directory]
# Examples
ls          # lists files in current directory
ls -l       # lists files with detailed information (permissions, owner, size, date)
ls /home    # lists files in /home directory
ls -a       # lists all files including hidden files (starting with .)

ls is used for listing files and directories. By default, it lists the current directory if no directory is specified.

## Pwd

# Definition:
pwd stands for “print working directory.” It shows the absolute path of the current working directory.

# Usage
Use pwd to check our current location in the file system.
# Formula
pwd

# Examples
bash

pwd
output might be: /home/username/labs
to check current directory before listing its contents
pwd
ls

## cd
# Definition:
cd (change directory) is used to move between directories in the file system.

# Usage:
we can navigate using absolute paths (full path from root) or relative paths (from our current location).

# Formula: 
cd [path-to-directory]
# Examples
bash
.Move to an absolute path
 cd /home/username/Documents
.Move to a subdirectory inside the current directory
cd Pictures
.Move up to the parent directory
cd ..
. Move to the home directory
cd ~

## Question 2
# Variable? 
A variable is a name that stores a value, such as text, numbers, or other data, which can be used later in commands or scripts.

# How to use a variable:
To use a variable, you assign it a value and reference it using $ before its name.

# Environment variable:
An environment variable is a variable that affects the behavior of the shell or system and is available to all programs and processes started from that shell.

# User-defined variable:
A user-defined variable is a variable created by the user to store information temporarily in the current session.

# Root directory:
The root directory is the top-most directory in the Linux file system hierarchy, represented by /.

# Parent directory:
The parent directory is the directory immediately above the current directory in the file system hierarchy.

# Current working directory:
The current working directory is the directory you are presently “in” in the shell.

# Absolute path:
An absolute path is the full path from the root directory to a file or folder.

# Relative path:
A relative path specifies a file or directory relative to your current working directory.

# Difference between “Your home directory” and “The home directory”:

Your home directory: The personal directory for your user account (e.g., /home/username).

The home directory: The general location where all users’ home directories are stored, usually /home.

## Question 3 
![img]