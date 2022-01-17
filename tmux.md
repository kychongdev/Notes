```bash
#Open new sessions from tmux
tmux new -s session_name

#Detach from tmux session
Ctrl+b d 

#List session
tmux ls

#Attach to session
tmux attach-session -t 0

Ctrl+b c            # create new window
Ctrl+b %            # split horizontally
Ctrl+b "            # split vertically
Ctrl+b 0            # switch to windows
Ctrl+b x            # close current pane
Ctrl+b (→, ←, ↑, ↓) # move between panel
```