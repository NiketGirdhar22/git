# Git Commands

## Why Use Git Commands?
These Command Line Interface (CLI) commands are used for various purposes instead of using the web interface:
- Tracking changes
- Saving changes
- Sharing changes with others

---

## Basic Git Commands

### Initializing a Git Repository
```sh
git init  # Creates a new repository and sets up all the necessary files and data structures for version control.
```

### Adding Files to Staging Area
```sh
git add <filename>  # Adds a specific file from the working directory to the staging area.
git add .           # Adds all modified and new files from the working directory to the staging area.
git add -A          # Stages all changes (including deletions) from the working directory.
```

### Committing Changes
```sh
git commit -m "commit message"  # Takes a snapshot of the changes in the staging area and stores it with a descriptive message.
```

### Viewing Commit History
```sh
git log  # Displays all previous commits along with their commit messages.
```

---

## Branching in Git

### Creating and Managing Branches
```sh
git branch                # Lists all the current branches in the repository.
git branch <branch_name>  # Creates a new branch with the specified name.
git branch -d <branch_name>  # Deletes the specified branch.
```

### Switching Between Branches
```sh
git checkout main  # Switches to the main branch.
git checkout <branch_name>  # Switches to another branch.
git switch <branch_name>  # Alternative command for switching branches.
```

### Checking Branch Status
```sh
git status  # Provides information about the currently used branch and the state of the files in relation to the repository.
```

### Merging Branches
```sh
git merge <branch_name>  # Merges the specified branch into the currently active branch.
```

---

## Remote Repository Commands

### Cloning a Repository
```sh
git clone <repository URL>  # Creates a local copy of a remote repository.
```

### Fetching and Merging Changes from Remote Repository
```sh
git pull origin main  # Fetches changes from the remote main branch and merges them into the local branch.
```

### Pushing Local Changes to Remote Repository
```sh
git push origin <branch-name>  # Pushes local commits to the specified remote branch.
```

### Managing Remote Repositories
```sh
git remote                # Lists all remote repositories connected to the local repository.
git remote -v             # Lists remote repositories along with their URLs.
git remote add origin <URL>  # Adds a remote repository with the specified URL.
git remote rename origin upstream  # Renames the remote repository from "origin" to "upstream."
git remote rm <name>  # Removes the specified remote repository.
```

---

## Resetting and Reverting Changes

### Resetting Changes
```sh
git reset  # Unstages changes but keeps working directory files.
git reset --hard HEAD  # Resets working directory and staging area to the last commit.
```

### Reverting Commits
```sh
git revert HEAD  # Creates a new commit that undoes the changes from the last commit.
```

---

## Additional Git Commands

### Viewing Differences Between Commits
```sh
git diff  # Shows differences between working directory and last commit.
git diff HEAD~1 HEAD  # Compares the last and second-last commits.
git diff <branch-1> <branch-2>  # Compares two branches.
```

### Configuring Git User Information
```sh
git config --global user.email "your-email@example.com"  # Sets a global email for Git.
git config --global user.name "Your Name"  # Sets a global username for Git.
```

### Viewing Git Version
```sh
git version  # Displays the installed Git version.
```

### Generating Patches
```sh
git format-patch HEAD~3  # Creates patches for the last three commits.
```

### Applying Patches
```sh
git am <patchfile.patch>  # Applies changes from a patch file.
```

### Sending Patches via Email
```sh
git send-email *.patch  # Sends multiple patch files as emails.
```

### Starting a Git Server
```sh
git daemon --base-path=/path/to/repositories  # Exposes repositories via the Git protocol.
```

### Launching a Web Interface for Repositories
```sh
git instaweb --httpd=webrick  # Instantly launches a web server to browse repositories.
```

### Resolving Merge Conflicts Automatically
```sh
git rerere  # Reuses recorded resolutions of previously resolved merge conflicts.
```