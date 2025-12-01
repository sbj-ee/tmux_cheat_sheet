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
CTRL +b$
</code>

detatch from session
<code>
CTRL +b d
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
CTRL +b (
</code>

change to next session
<code>
CTRL +b )
</code>

