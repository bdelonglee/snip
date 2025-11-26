#### GIT IVY
 ## commit all  push  Rsync Box207
com=""; echo "\033[1;33m\nGIT commit \n\033[0m"; git commit -a -m \"$com\"; echo "\033[1;33m\nGIT push  \n\033[0m"; git push; echo "\033[1;33m\nRSync box207  \n\033[0m"; rsync  -av --exclude="*.svg" ~/Documents/PROJECTS/DEV/ivy bdelonglee@box207:/u/hqr/FILM/WORK/SUP_SHELL_SCRIPTS/prod/ ; echo "\n\033[1;33m\Rsynced at \033[0m"; date '+%H:%M:%S'



# GIT SNAPSHOTS Initialize a Repository
git init


#### GIT SNAPSHOTS Staging files


#### GIT SNAPSHOTS Staging files
git add file1.js file2.js 


#### GIT SNAPSHOTS Staging files Pattern
## Stage with pattern
git add *.js 


#### GIT SNAPSHOTS Staging directory
## Stage the current dorectory and all its content
git add .


#### GIT SNAPSHOTS Viewing Full status
## Full Status
git status # Full status


#### GIT SNAPSHOTS Viewing Short status
## Short Status
git status -s


#### GIT SNAPSHOTS Committing the staged files
## Commit Classic Commits with a one-line message
git commit -m “Message” 


#### GIT SNAPSHOTS Committing the staged files
## Commit Open Editor
git commit 


#### GIT SNAPSHOTS Skipping the staging area
## Skipping Staging Area
git commit -am

#### GIT SNAPSHOTS Removing files (Work & Stage)
## Removes from working directory and staging area
git rm file1.js 


#### GIT SNAPSHOTS Removing files (Staging only)
## Removes from staging area only
git rm --cached file1.js 


#### GIT SNAPSHOTS Renaming or moving files
git mv file1.js file1.txt


#### GIT SNPASHOTS DIFF Viewing the staged/unstaged changes
## Shows unstaged changes
git diff 


#### GIT SNPASHOTS DIFF Viewing Staged Changes
## Show staged changes
git diff --staged 


#### GIT SNPASHOTS DIFF Viewing Staged Changes
## Same as the above
git diff --cached 


#### GIT SNAPSHOTS Viewing the history (Full)
## Full History
git log 


#### GIT SNAPSHOTS Viewing the history (Summary)
## Summary History
git log --oneline


#### GIT SNAPSHOTS Viewing the history (Graph)
## Graph History
git log --oneline --all --graph


#### GIT SNAPSHOTS Viewing the history (Reverse)
## Lists the commits from the oldest to the newest
git log --reverse


#### GIT SNAPSHOTS Viewing a commit
## Shows the given commit
git show 921a2ff


#### GIT SNAPSHOTS Viewing last commit
## Shows the last commit
git show HEAD

 
#### GIT SNAPSHOTS Viewing Steps before last commit
## Shows Two steps before the last commit
git show HEAD~2


#### GIT SNAPSHOTS Viewing File in last commit
## Shows the version of file.js stored in the last commit
git show HEAD:file.js


#### GIT SNAPSHOTS Unstaging files (undoing git add)
## Copies the last version of file.js from repo to index
git restore --staged file.js


#### GIT SNAPSHOTS Discarding local changes
## Copies file.js from index to working directory
git restore file.js


#### GIT SNAPSHOTS Discarding local changes
## Restores multiple files in working directory
git restore file1.js file2.js


#### GIT SNAPSHOTS Discarding local changes
## Discards all local changes (except untracked files)
git restore .


#### GIT SNAPSHOTS Discarding local changes
## Removes all untracked files
git clean -fd

#### GIT SNAPSHOTS Restoring an earlier version of a file
git restore --source=HEAD~2 file.js


#### GIT HISTORY Viewing the history
## Shows the list of modified files
git log --stat


#### GIT HISTORY Viewing the history
## Shows the actual changes (patches)
git log --patch

#### GIT HISTORY Filtering the history
## CMD
git log -3 
git log --author=“Mosh”
git log --before=“2020-08-17”
git log --after=“one week ago”
git log --grep=“GUI”           # Commits with “GUI” in their message
git log -S“GUI”                # Commits with “GUI” in their patches
git log hash1..hash2           # Range of commits
git log file.txt               # Commits that touched file.txt



#### GIT HISTORY Formatting the log output
#### GIT HISTORY Creating an alias
#### GIT HISTORY Viewing a commit
#### GIT HISTORY Comparing commits
#### GIT HISTORY Checking out a commit
#### GIT HISTORY Finding a bad commit
#### GIT HISTORY git shortlog
#### GIT HISTORY Finding the author of lines
#### GIT HISTORY Tagging
#### GIT BRANCHING Managing branches
#### GIT BRANCHING Comparing branches
#### GIT BRANCHING Stashing
#### GIT BRANCHING Merging
#### GIT BRANCHING Viewing the merged branches
#### GIT BRANCHING Rebasing
#### GIT BRANCHING Cherry picking
#### GIT COLLABORATION Cloning a repository
#### GIT COLLABORATION Syncing with remotes
#### GIT COLLABORATION Sharing tags
#### GIT COLLABORATION Sharing branches
#### GIT COLLABORATION Managing remotes
#### GIT REWRITING HISTORY Undoing commits
#### GIT REWRITING HISTORY Reverting commits
#### GIT REWRITING HISTORY Recovering lost commits
#### GIT REWRITING HISTORY Amending the last commit
#### GIT REWRITING HISTORY Interactive rebasing


#### GIT delete all merged remote branches EXCEPT main
git branch -r --merged main | grep -v "main" | sed 's/origin\///' | xargs -I {} git push origin --delete {}






