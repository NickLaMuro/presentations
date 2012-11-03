---
title: tmux-attach-detach-cont
category: vim-tmux
tags: ['content']
---

Tmux:  Attach and Detach
------------------------

* To enter tmux, you can just type `tmux` from the command line

  * This will attach you to a new session that is created with the name of '0'
    (creative, I know)

  * If you want name it yourself, use `tmux new -s [name_of_session]`

* To leave a session, just close it by typing `exit` in the last open pane

* To detach without closing a session type `Ctrl-b d` or `tmux detach`

* To attach to an existing session, use `tmux attach -t [name_of_session]`

  * To see a list of the open sessions, you can type `tmux list-sessions` or
    `tmux ls` from outside of a tmux session
