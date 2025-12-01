# tmux cheat sheet
## Sessions
Start a new session with the name *mysession*<br>
<code>tmux new -s mysession</code>

kill/delete session *mysession*<br>
<code>tmux kill-session -t mysession</code>

kill/delete all sessions except the current session<br>
<code>tmux kill-session -a</code>

kill/delete all sessions except *mysession*<br>
<code>tmux kill-session -a -t mysession</code>

rename session<br>
<code>CTRL+b $</code>

detatch from session<br>
<code>CTRL+b d</code>

show all sessions<br>
<code>tmux ls</code>

attach to last session<br>
<code>tmux a
tmux at
tmux attach
tmux attach-session</code>

attach to a session named *mysession*<br>
<code>tmux -a -t mysession
tmux attach-session -t mysession</code>

change to previous session<br>
<code>CTRL+b (</code>

change to next session<br>
<code>CTRL+b )</code>

## Windows
start a new session with the name *mysession* and window *mywindow*<br>
<code>tmux new -s mysession -n mywindow</code>

create window<br>
<code>CTRL+b c</code>

rename current window<br>
<code>CTRL+b ,</code>

close current window<br>
<code>CTRL+b &</code>

previous window<br>
<code>CTRL+b p</code>

next window<br>
<code>CTRL+b n</code>

switch/select window by number<br>
<code>CTRL+b 0 ... 9</code>

reorder window, swap number 2 (src) and 1 (dst)<br>
<code>swap-window -s 2 -t 1</code>

move current window to the left by one position<br>
<code>swap-window -t -1</code>

## Panes
toggle last active pane<br>
<code>CTRL+b ;</code>

split pane vertically<br>
<code>CTRL+b %</code>

split pane horizontally<br>
<code>CTRL+b "</code>

move the current pane left<br>
<code>CTRL+b {</code>

move the current pane right<br>
<code>CTRL+b }</code>

toggle synchronize-panes (send commands to all panes)<br>
<code>setw synchronize-panes</code>

toggle between pane layouts<br>
<code>CTRL+b SPACEBAR</code>

switch to next pane<br>
<code>CTRL+b o</code>

show pane numbers<br>
<code>CTRL+b q</code>

switch/select pane by number<br>
<code>CTRL+b q 0 ... 9</code>

toggle pane zoom<br>
<code>CTRL+b z</code>

convert pane into a window<br>
<code>CTRL+b !</code>

close current pane<br>
<code>CTRL+b x</code>

## Copy Mode
use vi keys in buffer<br>
<code>setw -g mode-keys vi</code>

enter copy mode<br>
<code>CTRL+b [</code>

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

go to last line
<code>
G
</code>

move cursor left
<code>
h
</code>

move cursor down
<code>
j
</code>

move cursor up
<code>
k
</code>

move cursor right
<code>
l
</code>

move cursor forward by word
<code>
w
</code>

move cursor backword by word
<code>
b
</code>

search forward
<code>
/
</code>

search backward
<code>
?
</code>

next keyword occurrence
<code>
n
</code>

previous keyword occurrence
<code>
N
</code>

start selection
<code>
SPACEBAR
</code>

clear selection
<code>
ESC
</code>

copy selection
<code>
ENTER
</code>

paste contents of buffer_0
<code>
CTRL+b ]
</code>

display buffer_0 contents
<code>
show-buffer
</code>

copy entire visible contents of pane to buffer
<code>
capture-pane
</code>

show all buffers
<code>
list-buffers
</code>

show all buffers and paste selected
<code>
choose-buffer
</code>

save buffer contents to *buf.txt*
<code>
save-buffer buf.txt
</code>

delete buffer_1
<code>
delete-buffer -b 1
</code>

## Miscellaneous
enter command mode
<code>
CTRL+b :
</code>

set OPTION for all sessions
<code>
set -g OPTION
</code>

set OPTION for all windows
<code>
setw -g OPTION
</code>

show every session, window, pane
<code>
tmux info
</code>

show shortcuts
<code>
CTRL+b ?
</code>
