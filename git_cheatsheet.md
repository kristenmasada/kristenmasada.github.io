---
layout: page
title: Git Cheatsheet
---

# Git Cheatsheet

_Last updated: 06/03/18_

* `git diff` - shows changes to files that will be tracked by Git when added.
* `git log` - history of commits.
  * `git log --graph --decorate --all` 

* `git reset --hard <commit>` - revert code back to a previous commit.
  * `<commit>` is the hash number for the commit; find using `git log`.
* `git reset --hard origin/master` - revert code back to the version on the remote repo (use if you want to discard all changes made since last pull).

* `git branch` - show all branches.
* `git branch <branch_name>` - create new branch.
* `git checkout <branch_name>` - switch to specified branch.
* `git checkout -b <branch_name>` - create branch + switch to it.
* `git merge <branch_name>` - merge branch `<branch_name>` with current branch.
* `git branch -D <branch_name>` - delete branch.
