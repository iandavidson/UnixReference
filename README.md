# UnixReference
Unix Reference

* pwd: present working directory
* mkdir: make directory
* ls: list directory contents
 * ls -FC: adds "/" for directories
 * ls -lt: long listing by recent time
* man: manual/help page for any command
 * man ls
* touch: either creates new empty file or updates last modified date on existing file
* repeating previous commands
 * !
 * up arrow
 * history: gives numbered list of previous commands, usable with ! command
   * !29 
* cd: change directory
 * cd <directory name>: into <directory name>
 * cd .. : takes to parent directory
 * cd ../.. : takes to grandparent directory
 * cd with no arguments takes to home directory
* more: displays text file while showing 1 page at a time
 * "spacebar": moves display forward one page/one page down
 * "b": moves display back one page
 * "return" : moves one line at a time
* cat : Concatenate multiple files together
 * cat file1 file2
* ^ : used to exchange text in command line
 * ^cat^more^ 
 * ^.java^.md^
* grep : search lines of file based on given pattern
 * grep cd README.md
 * grep ls README.md
 * grep cd *.md : converts *.md into all files that end in ".md"
 * grep -i cd *.md : makes search for "cd" not case sensitive
 * grep -i cd *.md file1.txt *.java : looks for "cd" non case sensitive in all files in directory ending with ".md", ".java" and the file named "file1.txt"
 * grep -i cd *.md file1.txt *.java | more : takes output and sends to more command
 * grep -i cd *.md file1.txt *.java > output : writes results to file in local directory named "output"
* find . -name *.java : gives list of all java files in all directorys below current location
 * find . -name "*.java" : if files in current directory match pattern, you must put the pattern in quotes
