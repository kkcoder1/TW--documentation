
# Git – Version Control System

## 1. Introduction

Git is a free and open-source distributed version control system used to track changes in files and manage source code.

It allows multiple developers to work on the same project while maintaining a history of changes.

Git was created by Linus Torvalds in 2005.

### Uses of Git

- Tracking changes in source code.
- Managing different versions of a project.
- Collaborating with other developers.
- Recovering previous versions of files.
- Managing software development workflows.

## 2. Features of Git

1. Distributed version control.
2. Fast performance.
3. Branching and merging.
4. Change tracking.
5. Offline working support.
6. Collaboration support.
7. Maintaining project history.

## 3. Installing Git

### Linux (Ubuntu)

```bash
sudo apt update
sudo apt install git
```

### macOS

```bash
brew install git
```

### Windows

Download Git from:

https://git-scm.com/downloads

### Verify Installation

```bash
git --version
```

## 4. Configuring Git

Before using Git, configure your username and email.

```bash
git config --global user.name "Your Name"

git config --global user.email "your-email@example.com"
```

To view the configuration:

```bash
git config --list
```

These details are used to identify the author of commits.

## 5. Creating a Repository

A Git repository stores project files and their version history.

To initialize a repository:

```bash
git init
```

This creates a hidden `.git` directory containing repository information.

To check repository status:

```bash
git status
```

## 6. Basic Git Workflow

Git uses three important areas:

1. Working Directory – Where files are created and modified.
2. Staging Area – Where changes are prepared for committing.
3. Repository – Where committed snapshots are stored.

### Basic Workflow

```bash
git add filename
git commit -m "Initial commit"
```

To add all modified and untracked files:

```bash
git add .
```

To check changes:

```bash
git status
```

## 7. Important Git Commands

| Command | Purpose |
|---|---|
| git init | Initializes a repository |
| git clone | Copies an existing repository |
| git status | Displays current status |
| git add | Adds changes to staging |
| git commit | Saves a snapshot |
| git log | Displays commit history |
| git diff | Shows unstaged changes |
| git branch | Lists branches |
| git checkout | Switches branches |
| git merge | Combines branches |
| git pull | Downloads and integrates changes |
| git push | Uploads local commits |
| git remote -v | Displays remote repositories |

## 8. Understanding Commits

A commit represents a saved snapshot of the project's staged changes.

Each commit contains information such as:

- Commit ID.
- Author.
- Date and time.
- Commit message.
- Changes included in the snapshot.

### Creating a Commit

```bash
git add .
git commit -m "Added documentation"
```

### Viewing Commit History

```bash
git log
```

For a compact history:

```bash
git log --oneline
```

Good commit messages should briefly describe the changes made.

## 9. Branching in Git

A branch is an independent line of development.

It allows developers to work on new features without directly modifying the main branch.

### Creating a Branch

```bash
git branch feature
```

### Switching Branches

```bash
git switch feature
```

### Creating and Switching Together

```bash
git switch -c feature
```

### Merging Branches

First switch to the branch that should receive the changes:

```bash
git switch main
git merge feature
```

### Deleting a Branch

```bash
git branch -d feature
```

## 10. Git Remote Repositories

A remote repository is a version of your project hosted on another server, such as GitHub.

### Adding a Remote

```bash
git remote add origin https://github.com/username/repository.git
```

### Viewing Remotes

```bash
git remote -v
```

### Uploading Changes

```bash
git push -u origin main
```

The `-u` option sets the upstream branch for future pushes.

After the initial push, you can generally use:

```bash
git push
```

## 11. Git Clone, Pull and Push

### Git Clone

Downloads an existing remote repository.

```bash
git clone https://github.com/username/repository.git
```

### Git Pull

Fetches and integrates changes from a remote repository.

```bash
git pull origin main
```

### Git Push

Uploads local commits to a remote repository.

```bash
git push origin main
```

## 12. Resolving Merge Conflicts

A merge conflict occurs when Git cannot automatically combine changes from different branches.

### Basic Resolution Steps

1. Run the merge command.
2. Identify the files containing conflicts.
3. Open the conflicting files.
4. Review both versions of the changes.
5. Edit the file to keep the intended content.
6. Stage the resolved file.
7. Create a commit if required.

## 13. Advantages of Git

- Tracks changes efficiently.
- Maintains complete project history.
- Supports teamwork.
- Allows parallel development through branches.
- Helps recover earlier versions.
- Supports distributed development.

## 14. Best Practices

- Write meaningful commit messages.
- Commit changes regularly.
- Check status before committing.
- Avoid committing unnecessary files.
- Use branches for new features.
- Pull updates before starting collaborative work.
- Keep the repository organized.

## 15. What I Learned

Through Git, I learned how version control systems help manage software projects.

I understood how to initialize repositories, stage files, create commits, manage branches and work with remote repositories.

Git is an essential tool for developers because it provides an organized way to track and manage changes.

## 16. Further Reading

- Official Git Website: https://git-scm.com/
- Git Documentation: https://git-scm.com/doc
