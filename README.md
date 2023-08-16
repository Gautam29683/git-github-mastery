## Setup Git and GitHub Global Configuration ##
$ git config --global user.email "gautamthakur1983@gmail.com"
$ git config --global user.name "Gautam Thakur"
$ git config --global list
$ git config --list

## Git Lifecycle ## Initilize, Status, Add, Commit
$ git status
$ git init
$ git add .
$ git commit -m "Commit Message"
$ git log 
$ git log --oneline

## Git Difference between last commit changes and current version changes ##
$ git diff

## Compare between 2 different Git Commits ##
$ git diff eac4c5b 82485b1

## Git Statsh - To save some changes for temporary purpose ## Pop take out stash and clear but apply take out stash but not clear
$ git stash (to save current changes for temporary)
$ git stash pop (to take out all stash contents)
$ git stash list
$ git stash clear (to clear all the stash changes)
$ $ git stash save "name" | $ git stash save "about" (working with multiple stash)
$ git stash apply 0 or 1 (0 for name, 1 for about) after that $ git stash clear

## Git Restore - It help us to restore previous state/commit or remove the changes we did ##
$ git restore FILENAME (restore all the changes in the working directory) It work for the indivisual file.
$ git restore --staged FILENAME (restore all changes from staging area)

## Git Branch - Creating, Deletion, Merging etc. ##
$ git branch (list all tghe branches)
$ git branch <NEW_BRANCH_NAME> (Create a new branch)
$ git checkout <BRANCH_YOU_WANT_TO_USE> (to change to the branch)








