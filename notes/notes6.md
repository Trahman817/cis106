# Notes 6
## mkdir

+ Definition:
  * Creates a new directory (folder) in the specified location.

+ Usage/Formula:
   * mkdir [directory-name]
+ Examples
    * mkdir myfolder
    * mkdir Documents/Work
    * mkdir -p a/b/c
  
## touch
+ Definition:
  * Creates an empty file or updates the timestamp of an existing file.

+ Usage/Formula:
   * touch [file_name]
+ Example
   * touch notes.txt
   * touch file1 file2 file3
   * touch -c oldfile.txt
## rm
+ Definition:
  * Removes (deletes) files or directories.

+ Usage/Formula:
   * rm [option] [file_or_directory]
+ Examples
   * rm file.txt
   * rm -i file.txt
   * rm -r myfolder
   * rm -rf myfolder
## cp
+ Definition:
  * Copies files or directories from one location to another.

+ Usage/Formula:
   * cp [options] [destination]
+ Examples
   * cp file1.txt file2.txt
   * cp file.txt /home/user
   * cp -r folder1 folder2
## mv
+ Definition:
  *  Moves or renames files and directories.

+ Usage/Formula:
  * mv [sources] [destination]
+ Examples 
  * mv oldname.txt newname.txt
  * mv file.txt /home/user
  * mv folder1 folder2/