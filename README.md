# GitHub learning

## Setup Git and GitHub Global Configuration ##
```
$ git config --global user.email "gautamthakur1983@gmail.com"
$ git config --global user.name "Gautam Thakur"
$ git config --global list
$ git config --list
```

## Git Lifecycle ## Initilize, Status, Add, Commit
```
$ git status
$ git init
$ git add .
$ git commit -m "Commit Message"
$ git log 
$ git log --oneline
```

## Git Difference between last commit changes and current version changes ##
```
$ git diff
```

## Compare between 2 different Git Commits ##
```
$ git diff eac4c5b 82485b1
```

## Git Statsh - To save some changes for temporary purpose ## Pop take out stash and clear but apply take out stash but not clear
```
$ git stash (to save current changes for temporary)
$ git stash pop (to take out all stash contents)
$ git stash list
$ git stash clear (to clear all the stash changes)
$ $ git stash save "name" | $ git stash save "about" (working with multiple stash)
$ git stash apply 0 or 1 (0 for name, 1 for about) after that $ git stash clear
```

## Git Restore - It help us to restore previous state/commit or remove the changes we did ##
```
$ git restore FILENAME (restore all the changes in the working directory) It work for the indivisual file.
$ git restore --staged FILENAME (restore all changes from staging area)
```
## Git Branch - Creating, Deletion, Merging etc. ##
```
$ git branch (list all tghe branches)
$ git branch <NEW_BRANCH_NAME> (Create a new branch)
$ git checkout <BRANCH_YOU_WANT_TO_USE> (to change to the branch)
$ git merge <UPDATED_BRANCH> (first checkout to main then merge with main)
$ git branch -d <FEATURE> (delete the new branch locally once you done with that)
$ git push origin --delete feature (delete the feature branch remotely on GitHub)
```

## Git Pull - Pull all the changes from the remote repository ##
```
$ git push origin main (to pull the changes from remote repository)
$ git config pull.ff false
``` 
> (in case you get any error while pulling the changes) https://stackoverflow.com/questions/62653114/how-can-i-deal-with-this-git-warning-pulling-without-specifying-how-to-reconci

## Git Merge Conflict ##


## Express commit - Only work if file is already staged once. It will not work for new file inside working area ##
```
$ git commit -a -m "COMMIT MESSAGE" or $ git commit -am "COMMIT MESSAGE"
```

## Create new branch and checkout at the same time ##
```
$ git checkout -b <NEW_BRANCH_NAME>
```

## Check all latest commit in all the branches ##
```
$ git branch -v
```

## Information about all the remote branches ##
```
$ git branch -r
```

## Check all the connected Remote Repository ##
```
$ git remote -v
```

## To check all the Merged and not Merged branches ##
```
$ git branch --merged
$ git branch --no-merged
```

## Delete the branch which is not merged with main ##
```
$ git branch -D filter (branch name)
```

## Git Rebase ## Rebase and Merge are use to integrate changes.
```
$ git rebase feature (Merge all the changes from feature to main, them rebase main to feature) 
$ git rebase main
```

## Git Rebase vs Git Merge ##
**Merge - Git merge keep history of everything. Have idea about conflicts**
**Rebase - Order of change not preserve in git rebase. No idea about merge conflict. After Rebase all the changes always added at the top. In spite of other commits in between. After Rebase, history on commit will be same with other branch.**

## Gitignore ##
