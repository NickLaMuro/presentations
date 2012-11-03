---
title: tmux-install-from-source
category: vim-tmux
tags: ['content']
---

Install from source
-------------------

* Linux prereqs

  * `$ sudo apt-get install build-essential`
  * `$ sudo apt-get install libevent-dev libncurses5-dev`

* Mac Prereqs:  XCode


Install Instructions:

    $ wget http://downloads.sourceforge.net/project/tmux/tmux/tmux-1.6/tmux-1.6.tar.gz
    $ tar -zxvf tmux-1.6.tar.gz
    $ cd tmux-1.6
    $ ./configure
    $ make
    $ sudo make install
