---
layout: page
title: Vim Cheatsheet
---

# Vim Cheatsheet

_Last updated: 05/26/18_

### File Navigation

#### [Command-T](https://github.com/wincent/command-t)
* `<Leader>t` - open Command-T.
  * note: `<Leader>` is mapped to `\` on my machine.
* `CTRL-S` - open selected file in horizontal split.
* `CTRL-V` - open selected file in vertical split.


#### [NERDTree](https://github.com/scrooloose/nerdtree)
* `:NERDTree` - open new NERDTree window for current directory.

##### File nodes
* `i` - open selected file in horizontal split.
* `gi` - preview in horizontal split.
* `s` - open in vertical split.
* `gs` - preview in vertical split.


### Splits

##### General
* `:sp`, `:split` - open horizontal split.
* `:vs`, `:vsplit` - open vertical split.
* `:q` - close current split.
* `:on`, `:only` - focus on current split (hides all other splits).
* `CTRL-W_{h,j,k,l}` - move cursor to another split.
  * note: might want to remap this to `CTRL_{h,j,k,l}` since I use this frequently.

##### Sizing
* note: for resizing splits, it is easiest to use autoresizing or the mouse in tmux.
* `CTRL-W_=` - make all splits a relatively equal size.
* `CTRL-W__` - 
* `CTRL-W_|` - 
* `CTRL-W_+` -
