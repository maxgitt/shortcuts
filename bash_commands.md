## Navigate and Edit Commandline
**go to**  
ctrl+a (start of line)  
ctrl+e (end of line)  
ctrl+&larr; (left one word)  
ctrl+&rarr; (right one word)  

**cut**  
ctrl+u (delete all left of cursor)  
ctrl+k (kill, delete all right of cursor)  
ctrl+w (kill word, delete one word left at a time)  

**paste**  
ctrl+y (yank back what has been cut)  
alt+. (paste previous argument) 

## Common Commands
**list all, one file per line, and classify**  
ll (ls -alF)  

**reverse search**  
ctrl+r "search term"  

**last command**  
!! (repeat last command, sudo !! is useful)  
!-3 (get third to last command)  
!^ (get first element of previous command line argument)  
!$ (get last element of previous command line argument)  
!:3 (get third element of previous command line argument  

**shell redirection**  
\> (file overwrite/creation)  
\>> (append to file)  

**kill terminal**  
reset  
ctrl+c  
ctrl+z, kill -9 (suspend to the background, then kill)  

## Search
**recursively look for files containing word**  
grep -rnw '/path/' -e 'word' (recursively, show line number, whole word)  
