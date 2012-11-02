---
title: vim-buffers-caveat
category: vim-tmux
tags: ['title']
---

Vim:  Buffers cont.
-------------------
One thing to keep in mind is that by default, vim won't let you switch between
buffers without saving the current buffer you are in first.  This gets old
pretty quick, and is not helpful when you are just using one file as a
reference.

To get around this, you can set the 'hidden' option (`:set hidden`) which will
let you swtich between buffers freely and keep your undo history for each.
