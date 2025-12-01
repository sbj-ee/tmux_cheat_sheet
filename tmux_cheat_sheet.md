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

