---
title: vim-find-and-replace-cont
category: vim-tmux
tags: ['content']
---

Vim:  Find and Replace
----------------------
* The syntax for find and replace:  `:%s/[existing-word]/[new-word]`

* You can add modifiers on to end of the expression

  * 'c' will require a confirmation with each substitution
  
  * 'g' will make the change globally on each line

  * 'i' ignores case (default) and 'I' is case sensitive

* Example:  To replace all instances of 'apple' with 'banana', type
  `:%s/apple/banana/g`
