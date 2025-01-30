# Git Commands

## Why use git commands?
These Command Line Interface [CLI] commands are used for various purposes instead of using the web interface
- Tracking changes
- Saving changes
- Sharing changes with others

---

## Basic git commands

- Initializing a git repository
```
git init
```
***This command reates a new repo and sets up all the necessary files and data structures for projects version control.***

- Adding files to staging area
```
git add <filename>
```
***This takes files/changes from working directory to staging are before commiting them. You can pass multiple files or use "." to select all files.***

- Commit the changes
```
git commit -m "commit message"
```
***This command takes a snapshot of the changes in the staging area and stores with a descriptive message.***

- View previous changes
```
git log
```
***This command is used to view all the previous commits recoreded along with their commit message.***

- Branching the repo
```
git branch <branch_name>
```
***This command creates a new branch with the branch_name and can be used to experiment with the code.***

- switching between branches
```
git checkout <branch_name> / git switch <branch_name>
```
***This command is used to switch to another branch in the repo.***

- Getting informantion about the branch
```
git status
```
***This command provides informantion about the currently used branch and the state of the files in relation to the repository***

- Getting information about the branch
```
git status
```
***This command shows the current branch you're on and provides the status of the files, including untracked, modified, and staged files, in relation to the repository.***

- Merging branches
```
git checkout main/master
git merge <branch_name>
```
***This first switches to the main/master branch and then merges the branch_name branch in the main/master branch***
[Note: It is a good practice to first use git pull command before using the merge command to avoid any conflicts when working with other collaborators]