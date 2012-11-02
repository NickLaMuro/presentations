---
title: vim-vimrc-keybindings
category: vim-tmux
tags: ['content']
---

.vimrc keybindings
------------------

* You are also able to create keybindings for the multiple modes of Vim in your
  .vimrc

* To create a command, you need three things:

  * The 'mapping' type: `map`, `nmap`, `vmap`, `imap`

  * The key combination

  * The command as you would enter it in normal mode

* Example to map 'F4' to `:bn`: `nmap <F4> :bn<CR>`

  * Non-alphanumeric keys usually are surrounded by `<` and `>`

  * `<CR>` stands for 'Carriage Return', or 'Enter'

