# Cloning VS Forking

## What is Cloning?
Cloning refers to creating a copy of a repository from a remote server (like GitHub) to your local machine. When you clone a repository, you get an identical copy of all the files, branches, and history from the remote repository. This allows you to work with the repository on your local system and push changes back to the original repository if you have the necessary permissions.

### Key Points:
- It copies the repository to your local system.
- You can make changes and push them to the original repository if you have write access.
- It's typically used to contribute directly to the project.

## What is Forking?
Forking is the process of creating a personal copy of someone else’s repository on GitHub. Unlike cloning, which copies the repository to your local machine, forking copies it to your GitHub account. This allows you to experiment and make changes freely without affecting the original repository. Forks are typically used when you want to contribute to a project but don't have write access to the original repository.

### Key Points:
- It copies the repository to your GitHub account.
- You can freely make changes without affecting the original repository.
- Typically used to propose changes via pull requests.

## Differences

| Feature | Cloning | Forking |
| ----- | ----- | ----- |
| **Where copied?** | Local machine | GitHub account |
| **Access** | Requires write access to the original repo | No need for write access to original repo |
| **Use case** | Directly contributing to the original repo | Contributing without write access |
| **Push changes** | Can push changes to original repo if allowed | Can push changes to forked repo |
| **Main action** | Copy and work locally | Copy to GitHub and propose changes |
| **Git Command** | `git clone <repository_url>` | Fork on GitHub, then `git clone <your_fork_url>` |
| **Where done?** | Locally on your machine | Done on GitHub interface |