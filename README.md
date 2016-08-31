# git-shortcuts
Git commands for .bashrc or .bash_profile for less typing

## Copy and paste

```bash

function searchCommits() {
  git log --all --oneline | grep $1
}

function archiveBranch() {
  git tag archive/$1 $1
  git branch -D $1
  git push origin --tags
}

alias pl='git pull --rebase'

alias gs='git status'

alias gf='git fetch'

```
