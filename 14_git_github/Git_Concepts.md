# Git Concepts

---

# 1. What is Git?

Git is a Distributed Version Control System (DVCS) used to track changes in source code and maintain the complete history of a project.

### Features

- Tracks source code changes
- Maintains project history
- Supports collaboration
- Allows rollback to previous versions
- Fast and lightweight

---

# 2. What is Version Control?

Version Control is the process of managing different versions of the same project over time.

Example:

Version 1
↓

Version 2
↓

Version 3
↓

Latest Version

If Version 3 contains a bug, Git allows us to restore Version 2.

---

# 3. What is GitHub?

GitHub is a cloud-based platform that hosts Git repositories.

### Uses

- Cloud Backup
- Team Collaboration
- Portfolio Creation
- Open Source Development
- Code Sharing

---

# 4. Git vs GitHub

Git

- Software
- Installed locally
- Works offline
- Tracks versions

GitHub

- Cloud Platform
- Stores repositories online
- Requires internet for synchronization

---

# 5. What is a Repository?

A Repository is the main project folder managed by Git.

Example

VLSI-Portfolio

Everything inside this folder is tracked by Git.

---

# 6. Working Directory

The Working Directory is the place where we create and modify project files.

Example

Git_Commands.md

---

# 7. Staging Area

The Staging Area temporarily stores selected changes before creating a commit.

Command

git add .

Purpose

Prepare files for the next commit.

---

# 8. Commit

A Commit is a snapshot of the current project.

Command

git commit -m "Added Git Notes"

Each commit contains

- Commit ID
- Commit Message
- Author
- Date and Time

---

# 9. Push

Push uploads local commits to GitHub.

Command

git push

---

# 10. Pull

Pull downloads the latest changes from GitHub.

Command

git pull

---

# 11. Repository Lifecycle

Create File
↓

Untracked
↓

git add .
↓

Staged
↓

git commit
↓

Committed
↓

git push
↓

GitHub

---

# 12. Git Diff

## Definition

Git Diff is used to compare the current version of a file with the last committed version.

It helps developers identify:
- Added lines
- Deleted lines
- Modified lines

## Command

```bash
git diff
```

## Example

Suppose the previous version contained:

Hello

Current version:

Hello
Welcome to Git

Git displays:

+ Welcome to Git

### Symbols

+ → Added line

- → Deleted line

## Uses

- Review changes before committing.
- Detect accidental modifications.
- Compare the current file with the previous commit.

---

# 13. Git Restore

## Definition

Git Restore restores a file to its last committed state.

It removes uncommitted changes.

## Command

```bash
git restore filename
```

Example

```bash
git restore README.md
```

## Uses

- Undo accidental edits.
- Restore files before committing.

Note:

Git Restore only affects uncommitted changes.

---

# 14. Git Branch

## Definition

A branch is an independent line of development.

It allows developers to work on new features or bug fixes without affecting the main project.

Main Branch

↓

Feature Branch

↓

Testing

↓

Merge

## Why Branches?

- Safe development
- Team collaboration
- Parallel development
- Bug fixing

---

# 15. Git Switch

## Definition

Git Switch changes the current working branch.

Example

```bash
git switch practice_branch
```

Return

```bash
git switch main
```

---

# 16. Git Remote

## Definition

Git Remote stores the information about the remote GitHub repository connected to the local repository.

Command

```bash
git remote
```

Example Output

origin

---

# 17. Git Remote -v

## Definition

Displays the URL of the connected GitHub repository.

Command

```bash
git remote -v
```

Example

origin https://github.com/Nikhilreddy0724/VLSI-Portfolio.git (fetch)

origin https://github.com/Nikhilreddy0724/VLSI-Portfolio.git (push)

---

# 18. Git Clone

## Definition

Downloads a repository from GitHub to a local computer.

Command

```bash
git clone repository_url
```

Used when:
- Setting up a new computer
- Downloading someone else's repository
- Starting an existing project