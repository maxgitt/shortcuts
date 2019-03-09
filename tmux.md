# Help
C-b ?

## Split screen  
C-b % (split vertical)  
C-b " (split horizontal)  

## Navigation
C-b <arrow> (move to pane)  

## Close pane
C-d  
exit  

## Window
C-b c (create new window)  
C-b p (prev window)  
C-b n (next window)  
C-b <number> (window number)  
  
## Resizing
C-b z (toggle full screen of a pane)  
C-b C-<arrow> (resize in direction of arrow)  
C-b , (rename current window)

## Sessions
tmux (start session)  
C-b d (detach session)  
C-b D (detach session and run as daemon)??  
tmux ls  
tmux attach -t <number>  
tmux new -s <name> (create session with name instead of default number)  
tmux rename-session -t <number> <database> (rename session from number to name)  

## Resurrect
https://github.com/tmux-plugins/tmux-resurrect
