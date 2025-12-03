# Notes 8
## cat
  +  Definition

      *  cat (concatenate) reads files and prints their content to the terminal. It can also combine multiple files and create new ones.

  + Usage / Formula
     *    Cat [OPTIONS] [FILE...]

  +  Examples
      *  Cat notes.txt (Displays the content of notes.txt.)

      *  Cat file1.txt file2.txt > combined.txt(Combines two files into one).

      *  Cat -n script.sh (Shows file contents with line numbers).


   ## tac
   +  Definition

      * tac is the reverse of cat. It prints file contents from bottom to top, line by line.

   +  Usage / Formula
       * tac [OPTIONS] [FILE]

  +  Examples
     *   tac logfile.txt (Displays a log file in reverse order.)


     *   tac list.txt > reversed.txt (Creates a reversed version of a file.)

##  head
  +  Definition

     *  head displays the first part of a file. By default, it shows the first 10 lines.

  +  Usage / Formula
     *  head [OPTIONS] [FILE]

  + Examples
    *  head songs.txt (Shows the first 10 lines.)


    *  head -n 5 data.csv (Shows the first 5 lines.)

    *  head -c 20 sample.txt (Shows the first 20 characters.)


## tail
  + Definition

    *   tail displays the end of a file. By default, it shows the last 10 lines. Often used for monitoring logs in real time.

  + Usage / Formula
    *  tail [OPTIONS] [FILE]

 +  Examples
    *  tail notes.txt (Shows the last 10 lines.)


    *  tail -n 3 emails.txt (Shows the last 3 lines.)

     * tail -f /var/log/syslog (Follows a file live as it updates.)


 ## cut
 +  Definition

    *   cut extracts columns, fields, or specific character ranges from a file.

  +   Usage / Formula
      * cut OPTION [FILE]


  * Common options:

    -d → delimiter

    -f → field number

     -c → character position(s)

  + Examples
    *  cut -d ',' -f 1,3 students.csv. (Extracts the 1st and 3rd comma-separated fields.)

     *  cut -c 1-5 words.txt. (Extracts characters 1 through 5 of each line.)


     *   cut -d ':' -f 1 /etc/passwd. (Displays only usernames from the passwd file.)


## sort
  + Definition

      *  sort arranges lines of a file alphabetically or numerically. It can also sort by specific fields.

  +  Usage / Formula
     *  sort [OPTIONS] [FILE]


  + Common options:

    -r → reverse order

    -n → numeric sort

    -k → sort by field

    -u → unique entries only

 +  Examples
    *  sort names.txt. (Sorts alphabetically.)


    * sort -n numbers.txt. (Sorts numerically.)


    *  sort -t ',' -k 2 students.csv. (Sorts numerically.)


## wc
 +  Definition

     * wc (word count) displays the number of lines, words, and characters in a file.

 + Usage / Formula
   *  wc [OPTIONS] [FILE]


 + Common options:

   -l → count lines

    -w → count words

    -c → count bytes/characters

 + Examples
   *  wc essay.txt. (Shows lines, words, and characters.)

   * wc -l logs.txt. (Counts lines only.)

   *  wc -w *.txt. (Counts words in all .txt files.)
  

