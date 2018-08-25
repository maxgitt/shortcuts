## Navigate and Edit Commandline
**go to** <br>
ctrl+a (start of line) <br>
ctrl+e (end of line) <br>
ctrl+&larr; (left one word) <br>
ctrl+&rarr; (right one word) <br>

**cut** <br>
ctrl+u (delete all left of cursor) <br>
ctrl+k (kill, delete all right of cursor) <br>
ctrl+w (kill word, delete one word left at a time)

**paste**  
ctrl+y (yank back what has been cut)  
alt+. (paste previous argument) 

## Common Commands
**list all, one file per line, and classify** <br>
ll (ls -alF) <br>

**reverse search** <br>
ctrl+r "search term" <br>

**last command** <br>
!! (repeat last command, sudo !! is useful) <br>
!-3 (get third to last command)
!^ (get first element of previous command line argument) <br>
!$ (get last element of previous command line argument) <br>
!:3 (get third element of previous command line argument <br>

**shell redirection** <br>
\> (file overwrite/creation) <br>
\>> (append to file)

## Search
**recursively look for files containing word** <br>
grep -rnw '/path/' -e 'word' (recursively, show line number, whole word)
