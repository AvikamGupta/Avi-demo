# Git & GitHub Notes

## What is Git?

Git is a **Version Control System (VCS)** that helps developers track changes in their code over time.

### Benefits of Git

* Tracks code changes.
* Maintains version history.
* Allows collaboration with other developers.
* Makes it easy to revert to previous versions.
* Integrates seamlessly with GitHub.

---

## What is GitHub?

GitHub is a cloud-based platform used to host Git repositories.

### Workflow

```text
Local Computer
      ↓
     Git
      ↓
   GitHub
```

---

# Installing and Configuring Git

## Check Git Version

```bash
git --version
```

---

## Configure Git (First Time Setup)

```bash
git config --global user.name "Your Name"

git config --global user.email "yourmail@gmail.com"
```

### Verify Configuration

```bash
git config --list
```

---

# Creating a Repository

## Initialize a Git Repository

```bash
git init
```

This command creates a new Git repository in the current directory.

---

# Checking Repository Status

```bash
git status
```

Displays:

* Modified files
* Untracked files
* Staged files

---

# Adding Files

## Add a Single File

```bash
git add filename.cpp
```

## Add All Files

```bash
git add .
```

---

# Creating Commits

## Save Changes

```bash
git commit -m "Added basic C++ notes"
```

A commit acts as a save point for your project.

---

# Viewing Commit History

## Detailed History

```bash
git log
```

## Short History

```bash
git log --oneline
```

---

# Connecting a Local Repository to GitHub

## Add Remote Repository

```bash
git remote add origin REPOSITORY_URL
```

Example:

```bash
git remote add origin https://github.com/username/repository-name.git
```

### Verify Remote

```bash
git remote -v
```

---

# Pushing Code to GitHub

## First Push

```bash
git branch -M main

git push -u origin main
```

## Future Pushes

```bash
git push
```

---

# Cloning a Repository

```bash
git clone REPOSITORY_URL
```

Example:

```bash
git clone https://github.com/username/project.git
```

---

# Pulling Latest Changes

```bash
git pull
```

Downloads and merges the latest changes from GitHub.

---

# Working with Branches

## Create a Branch

```bash
git branch feature
```

## Switch Branch

```bash
git checkout feature
```

### Modern Alternative

```bash
git switch feature
```

## Create and Switch to a Branch

```bash
git switch -c feature
```

---

# Useful Commands

## View All Branches

```bash
git branch
```

## View Remote Repositories

```bash
git remote -v
```

## View Tracked Files

```bash
git ls-files
```

---

# Daily Git Workflow

The most commonly used workflow is:

```bash
git status

git add .

git commit -m "Meaningful commit message"

git push
```

---

# Good Commit Messages

### Avoid

```bash
git commit -m "update"
```

### Prefer

```bash
git commit -m "Added loops notes"

git commit -m "Solved 5 array questions"

git commit -m "Created calculator project"
```

---

# Git Workflow Summary

```text
Modified File
      ↓
   git add
      ↓
  Staging Area
      ↓
 git commit
      ↓
 Local Repository
      ↓
   git push
      ↓
    GitHub
```

---

# Key Commands Cheat Sheet

| Task                  | Command                     |
| --------------------- | --------------------------- |
| Initialize Repository | `git init`                  |
| Check Status          | `git status`                |
| Add File              | `git add filename`          |
| Add All Files         | `git add .`                 |
| Commit Changes        | `git commit -m "message"`   |
| View History          | `git log --oneline`         |
| Add Remote            | `git remote add origin URL` |
| Push Code             | `git push`                  |
| Pull Changes          | `git pull`                  |
| Clone Repository      | `git clone URL`             |
| Create Branch         | `git branch branch-name`    |
| Switch Branch         | `git switch branch-name`    |

---

# Conclusion

Git is an essential tool for every developer. Learning Git and GitHub early helps in project management, collaboration, and maintaining a professional development workflow.
