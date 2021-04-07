# Command Line text editors
* linux offers a lot of command line toools for handling text.
* some are
  * Cat Tac More Les Head Diff Tail Cut Paste Sort Wc Tr Grep
 ## Cat
* used for displaying the content of a file
* short for concatenate which means joining two strings together.
* Usage) 
  * cat + file to display
  * cat + file1 + file2
![img2]

 ## Tac
* used to display content of file in reversed order in a line by line basis
* The Tac command also concatenate files in revere order
* Usage)
  * tac + file to display
  * tac + file1 + file2
![img3]
 ## More
* used to display the content of a text file one page at a time
* usage) 
  * more + file to view
* for getting help nav the menu press h
* ex) open a file 10 lines at a time
  * more -10 /var/log/syslog
## Less
* used to display less content at a time
* faster than more when dealing with large file
* ex) open file with line number
  * less -N /var/log/syslog
* ex) open file at the beginning of the first occurance of string
  * less -p "nobody" /ect/passwd
 ## Head
* displays the top N numbers of lines of file. default prints first 10 lines. 
* ex) display first 10 lines of a file
  * head /ect/passwd
* ex) display the first 5 lines of file
  * head -5 /etc/passwd
## Tail
* displays last N number of lines in file. default last 10 lines.
* ex) display last 10 lines 
  * tail /ect/passwd
* ex) display last 5 lines
  * tail -5 /ect/passwd.
## Cut
* used to extract a specific section of each line of file and display it on the screen.
## Paste
* used to join files horizontally in columns.
## Sort
* used for sorting files
* sorts content of text files in particular order.
* supported sorting:
  * Alphabetically 
  * In reverse order
  * by number
  * by month
* ex) sort file in reverse order
  * sort -r users.txt
## Wc 
* used for printing the number of lines, characters, and bytes ina file
## Tr
* used for  translating or deleting characters from standard output.
## Diff
* compares files and displays the difference between them.
## Grep
* used to match string patterns from file or standard output when using the pipe
## Rev
* used for reversing the characters position in a given text.


* 