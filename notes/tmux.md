## Tmux cheat sheet

### Sessions

1.  Start a new session

            tmux new -s <session-name>

2.  Attach to a session (from outside tmux)

            tmux attach -t <session-name>
            tmux a

3.  Detach from a session

            Press Ctrl+b, then d

4.  List sessions

            tmux ls

### Windows

We can have windows inside a session

1.  Create a new window

            Press Ctrl+b, then c

2.  Rename the current window:

            Press Ctrl+b, then ,

3.  Kill a window / session

            Press Ctrl+d

4.  Switch between sessions and windows

            Press Ctrl+b, then w
            Press Ctrl+b, then <window number>
            Press Ctrl+b, then p (previous window)
            Press Ctrl+b, then n (next window)

### Panes

In a window we can have multiple panes:

1.  Split horizontal

            Press Ctrl+b, then %

2.  Split vertically

            Press Ctrl+b, then "

3.  Switch between panes

            Press Ctrl+b, then <arrow keys>

4.  Close a pane

            Press Ctrl+b, then x

### More

1.  Rename session

            tmux rename-session -t <old-name> <new-name>

2.  Kill all sessions

            tmux kill-server

