---
title: tmux-config-change-prefix
category: vim-tmux
tags: ['content']
---

Tmux:  Configuration Cont.
--------------------------

* The default prefix key is also not that easy to use, and while it doesn't
  conflict with a whole lot, it still is nice to have a prefix key that is
  convenient to use.

* To change the prefix key, add the following to your `.tmux.conf`

    unbind C-b
    set -g prefix C-a
