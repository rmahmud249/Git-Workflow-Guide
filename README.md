# Git Workflow Guide

A simple step-by-step guide for creating a Git repository, working with branches, merging changes, and using common Git commands.

---

# 1. Create a Local Git Repository

Initialize a new Git repository.

```bash
git init
```

**Description:**
Creates a new local Git repository in the current folder.

---

# 2. Add Files

Stage all project files.

```bash
git add .
```

**Description:**
Adds all files to the staging area.

---

# 3. Commit Files

Save the staged changes.

```bash
git commit -m "Initial commit"
```

**Description:**
Creates the first commit.

---

# 4. Create a GitHub Repository

Create a new repository on GitHub.

Example:

```
https://github.com/username/project-name.git
```

---

# 5. Connect Local Repository to GitHub

```bash
git remote add origin <repository-url>
```

Example:

```bash
git remote add origin https://github.com/username/project-name.git
```

**Description:**
Connects your local repository with GitHub.

---

# 6. Push Main Branch

```bash
git push -u origin main
```

**Description:**
Uploads the **main** branch to GitHub and sets it as the default upstream branch.

---

# Branch Workflow

## 7. Create a New Branch

Method 1

```bash
git branch Branch-1
```

Creates a new branch.

OR

Method 2 

```bash
git switch -c Branch-1
```

Creates and switches to the new branch.

---

## 8. Switch to an Existing Branch

```bash
git switch Branch-1
```

Moves to **Branch-1**.

---

## 9. Make Changes

Edit your project files.

---

## 10. Stage Changes

```bash
git add .
```

Stages all modified files.

---

## 11. Commit Changes

```bash
git commit -m "Added new feature"
```

Saves the changes.

---

## 12. Push Branch to GitHub

```bash
git push -u origin Branch-1
```

Uploads the branch to GitHub.

---

# Merge Branch into Main

## 13. Switch Back to Main

```bash
git switch main
```

---

## 14. Merge Branch

```bash
git merge Branch-1
```

Merges **Branch-1** into **main**.

---

## 15. Push Updated Main

```bash
git push origin main
```

Uploads the merged changes.

---

# Delete Branch 

## Delete Local Branch

```bash
git branch -d Branch-1
```

Deletes the local branch.

---

## Delete Remote Branch

```bash
git push origin --delete Branch-1
```

Deletes the branch from GitHub.

---

# Useful Git Commands

| Command | Description |
|----------|-------------|
| `git status` | Show repository status |
| `git branch` | List local branches |
| `git branch -a` | List local and remote branches |
| `git log --oneline` | Show commit history (short format) |
| `git pull origin main` | Download and merge the latest changes |
| `git fetch` | Download remote changes without merging |
| `git remote -v` | Show connected remote repositories |
| `git checkout <branch>` | Switch branches (older command) |
| `git switch <branch>` | Switch branches (recommended) |

---

