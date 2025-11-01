## Notes 5

# ls
* # Definition:

  + ls lists files and directories in a folder.
* # Usage

     *  By default, ls lists the contents of the current directory. You can also specify a directory or file to list.
* # Formula

  * bash ls [options] [directory]
* # Examples

  * ls  lists files in current directory 
  * ls -l  lists files with detailed information (permissions, owner, size, date) 
  * ls /home  lists files in /home directory 
  * ls -a  lists all files including hidden files (starting with .)


## Pwd
 * # Definition:

   * pwd stands for “print working directory.” It shows the absolute path of the current working directory.
* # Usage

  * Use pwd to check our current location in the file system.
* # Formula

  * pwd
* # Examples



  * pwd output might be: /home/username/labs to check current directory before listing its contents pwd ls
## Cd
* #    Definition:

* cd (change directory) is used to move between directories in the file system.
* # Usage:

  * we can navigate using absolute paths (full path from root) or relative paths (from our current location).
* # Formula:

   *   cd [path-to-directory]
* # Examples

  *    bash .Move to an absolute path cd /home/username/Documents .Move to a subdirectory inside the current directory cd Pictures .
  *    Move up to the parent directory cd .. . Move to the home directory cd ~
