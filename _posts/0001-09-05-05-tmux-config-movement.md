---
title: tmux-config-change-movement
category: vim-tmux
tags: ['content']
---

Tmux:  Configuration Cont.
--------------------------

Movement in tmux also doesn't default to something that you are propbably
already comfortable with:  the Vim key bindings, so you can make some changes
to make using tmux similar to Vim

Change movement keys:

    bind h select-pane -L
    bind j select-pane -D
    bind k select-pane -U
    bind l select-pane -R

Change how you resize panes:

    bind-key J resize-pane -D 5
    bind-key K resize-pane -U 5
    bind-key H resize-pane -L 5
    bind-key L resize-pane -R 5

Change copy mode:  `set-window-option -g mode-keys vi`
