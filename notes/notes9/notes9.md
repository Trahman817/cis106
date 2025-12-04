# Notes 9
## 1. grep
+ Definition

  *  grep (Global Regular Expression Print) searches files or input for lines that match a pattern.

+ Usage / Formula
  *  grep [options] "pattern" filename

 + Examples
   * grep "error" logfile.txt (Search for lines containing the word “error”.)


   *  grep -i "warning" system.log. (Case-insensitive search.)


   *  ps aux | grep "firefox".(Search running processes for “firefox”.)



## 2. awk
 + Definition

   *   awk is a text-processing and pattern-scanning language used to manipulate data in lines and columns.

+ Usage / Formula
   *  awk 'pattern { action }' filename

+ Examples
  *  awk '{print $1}' employees.txt (Print the first column.)

   *  awk '/error/ {print $0}' server.log (Print lines containing the word “error”.)

  *  awk -F ":" '{print $1, $3}' /etc/passwd (Use : as a delimiter and print specific fields.)


## 3. sed
+ Definition

   *  sed (Stream Editor) performs editing operations on text, such as replacing, deleting, or inserting lines.

+ Usage / Formula
   * sed 'command' filename

+ Examples
   *  sed 's/apple/orange/' fruits.txt (Replace first occurrence of "apple" with "orange" on each line.)


   *  sed 's/error/ERROR/g' log.txt (Replace all occurrences.)


   *  sed '2d' data.txt (Delete line 2.)


# Pipes (|)
+ Definition

   *  A pipe sends the output of one command as the input of another command.

+ Usage / Formula
  *  command1 | command2

+ Examples
   * ls -l | grep ".txt" (Filter the list of files to only .txt files.)

   *  cat access.log | awk '{print $1}' (Show only the first column from a log file.)

+ ps aux | grep firefox | awk '{print $2}' (Find the process ID of Firefox.)


# Saving Output to a File (>)
+ Definition

   * The > operator redirects output to a file.
It overwrites the file if it already exists.

+ Usage / Formula
  *  command > filename

+ Examples
  *  ls > filelist.txt

  * grep "error" server.log > errors.txt

   * df -h > disk_usage.txt

# Appending Output to a File (>>)
+ Definition

   * The >> operator redirects output to a file but appends instead of overwriting.

+ Usage / Formula
   *  command >> filename

+ Examples
  *  echo "New log entry" >> output.log

   * grep "login" auth.log >> activity_report.txt

  *  date >> timestamps.txt
