# Git training

This project is git training with some immediate advanced commands.

## Basics

Here some 'quick' basic commands are listed

```bash
  # initialize git repo
  git init

  # add remote
  git remote add origin git@github.com:dmijatovic/git-practice-1.git

  # view remotes
  git remove -v

  # fetch changes from remote repo (get it to origin branches)
  git fetch

  # pull changes from remote repo into local branch
  git pull origin master

  # push changes
  git push origin master

```

## Git status and logs

```bash
  # show current status of repo
  git status

  # show basic changes
  git log

  # show changes using graph for all branches one line for each commit
  git log --oneline --graph --all

```

## Git commit (save changes)

When commit command is issued all files that are STAGED are committed to CURRENT branch the user is on. So this command depends on command to stage the files.

```bash

  # commit STAGED files
  git commit -m "This is my message"

  # commit STAGED and UNSTAGED files - BUT NOT UNTRACKED (new) files
  git commit -am "This is my message"

  # add all untracked files (or you can add by filename)
  git add .


```



## Comparing changes with Git

Use git diff command or difftool. (if defined)

### Define git difftool to be VSCode


## Rebasing in git

The common approach is to rebase feature/fix branch with the changes from the master. This will pull changes from master branch and then replay your changes on the top of it.

```bash

  # swith to feature branch
  git checkout feature

  # rebase feature branch with changes from master
  git rebase master

```