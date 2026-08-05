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
