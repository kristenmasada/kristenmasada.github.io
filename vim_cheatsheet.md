---
layout: page
title: Vim Cheatsheet
---

# Vim Cheatsheet

_Last updated: 06/26/18_

## Basic Text Manipulation
* `yy` or `Y` - copy a line.


## File Navigation

#### [Command-T](https://github.com/wincent/command-t)
* `<Leader>t` - open Command-T.
  * note: `<Leader>` is mapped to `\` on my machine.
* `CTRL-s` - open selected file in horizontal split.
* `CTRL-v` - open selected file in vertical split.
* `CTRL-t` - open selected file in tab.


#### [NERDTree](https://github.com/scrooloose/nerdtree)
* `:NERDTree` - open new NERDTree window for current directory.

##### File Nodes
* `i` - open selected file in horizontal split.
* `gi` - preview in horizontal split.
* `s` - open in vertical split.
* `gs` - preview in vertical split.


## Line Numbers
* `<Leader>r` - Cycle between relative line numbers, line numbers, and no line numbers.


## Movement
* `[number]{j,k}` - move <number> lines down or up.
* `CTRL-o` - go backward in jump list (go to previous location where cursor has been).
* `CTRL-i` - go forward in jump list.
* `H` - move cursor to top of file (high).
* `M` - move to middle of file (medium).
* `L` - move to bottom of file (low).
* `{` and `}` - jump between blank lines upward and downward in file.
* `CTRL-d` and `CTRL-u` - jump downward and upward in large chunks. 
* `CTRL-e` and `CTRL-y` - scroll downwar and upward without moving cusor. 


## Regular Expressions
* `*` - 0 or more (don't escape!).
* `\+` - 1 or more (need to escape).
* `\{x,y}` - ? (only escape opening bracket).
* `\( \)` - (escape both parens).
* note: to avoid dealing with weird escaping inconsistencies above, turn on 'very magic' mode (add `\v` after `/` when turning on search), so that everything is considered to be special unless escaped. Can map this so that it is always turned on when using search.


##### Lookahead/lookbehind
* `\zs` - match starts at this point (use for look behind).
* `\ze` - match ends at this point (use for look ahead). 


##### Case tricks
* `\C` - force search to be case sensitive.
* `\c` - force search to be case insensitive.
* note: I have `ignorecase` and `smartcase` turned on, meaning case is ignored if search term is all lower case, but case is considered when search term contains upper case letters. 
* `\u` - uppercase next letter in replacement. 
* `\l` - lowercase ".
* `\U` - uppercase replacement from here on (until \e or \E).
* `\L` - lowercase ".
* note: `:h regex` is very useful.


## Splits

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

## Tabs
* `CTRL-W_T` - convert current window/split to a tab.
* `:tabe [file]` - open new tab. if file provided, opens file in tab.
* `gt` and `gT` - go to next and previous tabs.

---
# Resources 
1. [Wincent's Vim Screencasts](https://www.youtube.com/playlist?list=PLUrFrOjgnsbZJNPvZkhsTRuuhYk1ArO0p)
