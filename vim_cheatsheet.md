---
layout: page
title: Vim Cheatsheet
---

# Vim Cheatsheet

_Last updated: 05/28/18_

### File Navigation

#### [Command-T](https://github.com/wincent/command-t)
* `<Leader>t` - open Command-T.
  * note: `<Leader>` is mapped to `\` on my machine.
* `CTRL-s` - open selected file in horizontal split.
* `CTRL-v` - open selected file in vertical split.
* `CTRL-t` - open selected file in tab.


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
* `CTRL-W_{h,j,k,l}` - move cursor to split to left/bottom/top/right.
  * note: might want to remap this to `CTRL_{h,j,k,l}` since I use this frequently.

##### Sizing
* note: for resizing splits, it is easiest to use [autoresizing](https://github.com/wincent/wincent/blob/c1a9be84f781b360219fb57613ffdd95c683c1b4/roles/dotfiles/files/.vim/plugin/autocmds.vim#L5) or the mouse.
* `CTRL-W_=` - make all splits a relatively equal size.
* `CTRL-W__` - maximize height of split. 
* `CTRL-W_|` - maximize width of split.
* `CTRL-W_+` and `CTRL-W_-` - increase and decrease height of split.
* `CTRL-W_>` and `CTRL-W_<` - increase and decrease width of split.

##### Movement
* `CTRL-W_{H,J,K,L}` - move split to left/bottom/top/right.

### Tabs
* `CTRL-W_T` - convert current window/split to a tab.
* `:tabe [file]` - open new tab. if file provided, opens file in tab.
* `gt` and `gT` - go to next and previous tabs.

---
# Resources 
1. [Wincent's Vim Screencasts](https://www.youtube.com/playlist?list=PLUrFrOjgnsbZJNPvZkhsTRuuhYk1ArO0p)
