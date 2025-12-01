# tmux cheat sheet
## Sessions
Start a new session with the name *mysession*
<code>
tmux new -s mysession
</code>

kill/delete session *mysession*
<code>
tmux kill-session -t mysession
</code>

kill/delete all sessions except the current session
<code>
tmux kill-session -a
</code>

kill/delete all sessions except *mysession*
<code>
tmux kill-session -a -t mysession
</code>

rename session
<code>
CTRL+b$
</code>

detatch from session
<code>
CTRL+b d
</code>

show all sessions
<code>
tmux ls
</code>

attach to last session
<code>
tmux a
tmux at
tmux attach
tmux attach-session
</code>

attach to a session named *mysession*
<code>
tmux -a -t mysession
tmux attach-session -t mysession
</code>

change to previous session
<code>
CTRL+b (
</code>

change to next session
<code>
CTRL+b )
</code>

## Windows
start a new session with the name *mysession* and window *mywindow*
<code>
tmux new -s mysession -n mywindow
</code>

create window
<code>
CTRL+b c
</code>

rename current window
<code>
CTRL+b ,
</code>

close current window
<code>
CTRL+b &
</code>

previous window
<code>
CTRL+b p
</code>

next window
<code>
CTRL+b n
</code>

switch/select window by number
<code>
CTRL+b 0 ... 9
</code>

reorder window, swap number 2 (src) and 1 (dst)
<code>
swap-window -s 2 -t 1
</code>

move current window to the left by one position
<code>
swap-window -t -1
</code>

## Panes
toggle last active pane
<code>
CTRL+b ;
</code>

split pane vertically
<code>
CTRL+b %
</code>

split pane horizontally
<code>
CTRL+b "
</code>

move the current pane left
<code>
CTRL+b {
</code>

move the current pane right
<code>
CTRL+b }
</code>

toggle synchronize-panes (send commands to all panes)
<code>
setw synchronize-panes
</code>

toggle between pane layouts
<code>
CTRL+b SPACEBAR
</code>

switch to next pane
<code>
CTRL+b o
</code>

show pane numbers
<code>
CTRL+b q
</code>

switch/select pane by number
<code>
CTRL+b q 0 ... 9
</code>

toggle pane zoom
<code>
CTRL+b z
</code>

convert pane into a window
<code>
CTRL+b !
</code>

close current pane
<code>
CTRL+b x
</code>

## Copy Mode
use vi keys in buffer
<code>
setw -g mode-keys vi
</code>

enter copy mode
<code>
CTRL+b [
</code>

enter copy mode and scroll one page up
<code>
CTRL+b PGUP
</code>

quit mode
<code>
q
</code>

go to top line
<code>
g
</code>

