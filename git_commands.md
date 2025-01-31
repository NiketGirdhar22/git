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
git init # creates a new repo and sets up all the necessary files and data structures for projects version control
```

- Adding files to staging area
```
git add <filename> # takes file/changes from working directory to staging area
git add . # takes all the files from working directory to staging area
git add -A # takes all the files from working directory to staging area
```

- Commit the changes
```
git commit -m "commit message" # takes a snapshot of the changes in the staging area and stores with a descriptive message
```

- View previous changes
```
git log # used to view all the previous commits recoreded along with their commit message
```

- Branching the repo
```
git branch # lists all the current branches in the repo
git branch <branch_name> # creates a new branch with the branch_name and can be used to experiment with the code
git branch -d <branch_name> # deletes branch_name
```

- switching between branches
```
git chechout main / git switch main # switches to the main branch of the repo
git checkout <branch_name> / git switch <branch_name> # switches to another branch in the repo
```

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