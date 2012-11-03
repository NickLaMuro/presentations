---
title: tmux-config-quick-reload
category: vim-tmux
tags: ['content']
---

Tmux:  Configuration Cont.
--------------------------

We are about to make a lot of changes to the `.tmux.conf`, and restarting tmux
everytime is no picnic.  To make this easier, we can reload tmux by running the
following command:

    source-file ~/.tmux.conf

This is similar to reloading your `.bashrc` when you make changes.  To make
this even easier, you can bind this to a key mapping:

    bind-key r      source-file ~/.tmux.conf; display-message "~/.tmux.conf is reloaded"
