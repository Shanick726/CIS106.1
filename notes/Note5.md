# Command Line text editors
## Basics of Nano 

* Can be open by typing nano
* to get help CTRL+G to get help
* CTRL+O to save
* to exit CTRL+X
* to open already existing file type "nano (file name)"
* open file with in nano CTRL+R 
* to copy data ALT+A to select data and copy ALT+^
* to paste CTRL+U
* to cut CTRL+K
* To move to top ALT \ 
* move to bottom ALT /
* ALT+G to find specific line number
* CTRL+W to look for string.
* ALT+R to replace word
* CTRL Y for page up CTRL V for page down

## Basics of VIM
Vim is not included in Ubuntu.
* Start by typing Vim 
* to quit hit esc and type :qa
  * : -> prefix for entering command line mode
  * q -> short for quit
  * a -> short for all buffers
  * ! -> force 
  * :qa! -> quit all
  * w -> saves
* set line numbers -> :set number
**Vim Modes:** 
* **Insert mode:** 
* **Normal mode:**used for manipulating text
  * Navigating file
    * H = left
    * J = down
    * k= up
    * l = right
* **Command mode:**used for writing text
*  **Visual mode:** used for navigation and manipulation of text selections
*  **Select mode:** similar to visual mode
*  **Ex-mode:** Similar to command-line mode but optimized for batch processing.
   *  when you start vim you are in normal
   *  press i to go to insert mode
   *  to switch back to normal hit esc or ctr+c
* edit by entering e "fileName"
### Moving around words in a file
* to move between words use w e
  * w -> moves word by word to the beginning of each word
  * e -> moves word by word at the end of each sentence.
    * 10e will move 10 words
  * To move between sentences use ()
    * ( -> previous sentence
    * ) -> next sentence
  * To move between paragraphs use {}
    * { -> previous paragraph
    * } -> next paragraph
### Searching words in vim
* use "/" and word 
  * ex) /Potato 
* N -> repeats search for the next word
* ? - > search backwards
* (*) -> will search for next occurrence of the word under the cursor
* (#) -> searches backwards for previous occurrence of the word under the cursor
  ### Screen Movement
  * G -> moves to end of file
  * gg -> moves ti beginning of file
  * CTRL+f -> moves a page forward at a time
  * CTRL+b -> moves a page back at a time
  * to move forward multiple pages use number "2 CTRL+f
  ### Moving lines 
  * to move to a specific line use : plus line number
    * :8 will move to line 8 
  * $ -> moves to end of line
  * 0 -> will move to beginning of line
### Delete text and copy and paste
* dw = delete current word
* u = undo
* dd = delete line under curser
*  d + /word = delete until word given
*  yw = copy yhe current word
*  p = for paste after curser
*  P = paste before curser
*  yy = copies whole line
*  x = for cut
### Change text
* cw = deletes the word under the curser and enter insert mode
* c /hello = deletes until finds the word hello and enters insert mode
* Visual selection 
  * SHIFT + V  select line
  * CTRL + V selectd block
* Replace text
  * : s/oldW/newW = replace old word ofr new
  * : s/old/new = replaces the first occurrence of the word old
  * %s/old/new/g = replaces all occurrences of the word old
  * %s/old/new/g/y = will ask to replace word

# Handling text files 
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