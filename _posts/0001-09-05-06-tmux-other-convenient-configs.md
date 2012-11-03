---
title: tmux-other-convenient-configs
category: vim-tmux
tags: ['content']
---

Tmux:  Configuration Cont.
--------------------------

These are just a few more configs that are nice:

    set -g base-index 1    # start window index of 1

    set -sg escape-time 1  # fixes some delay issues in vim

    bind-key a      send-key C-a   # `Ctrl-a a` sends `Ctrl-a`
    bind-key n      command-prompt 'rename-window %%'
    bind-key N      command-prompt 'rename-session %%'
    bind-key -r <   swap-window -t :-
    bind-key -r >   swap-window -t :+

    # Copy mode keybindings
    unbind p
    bind p paste-buffer
    bind -t vi-copy 'v' begin-selection
    bind -t vi-copy 'y' copy-selection
