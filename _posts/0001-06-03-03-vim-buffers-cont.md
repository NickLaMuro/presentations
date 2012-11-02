---
title: vim-buffers-cont
category: vim-tmux
tags: ['content']
---

Vim:  Buffers
-------------
* Each file that is opened is kept in a buffer, and can be re-accessed at any
  point

* To switch between the buffers, you can type `:bp` and `:bn` to move to the
  previous and next buffers respectively

* To delete a buffer (close a file in Vim), you can type `:bd`.

  * This will close the split you are in as well if it is not the last split
    that is open

  * It will also not close vim if you close the last buffer, and will just take
    you to a empty file buffer
