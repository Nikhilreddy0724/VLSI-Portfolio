# Git Workflow

## Standard Workflow

Write Code
↓

git status

Checks modified files.

↓

git add .

Stages files.

↓

git commit -m "Meaningful Message"

Creates a checkpoint.

↓

git push

Uploads commits to GitHub.

---

## Industry Workflow

Developer

↓

Write RTL Code

↓

Compile

↓

Simulate

↓

Debug

↓

git status

↓

git add .

↓

git commit

↓

git push

↓

GitHub Repository

---

# Understanding Git Diff

Previous Commit
↓

Current Modified File

↓

git diff

↓

Displays Added (+) and Deleted (-) Lines

---

# Understanding Git Restore

Modified File

↓

git restore filename

↓

Last Committed Version Restored

---

# Branch Workflow

main

↓

git branch feature_branch

↓

git switch feature_branch

↓

Develop Feature

↓

git commit

↓

git switch main

↓

git merge feature_branch

---

# Remote Repository Workflow

Local Repository

↓

git push

↓

GitHub Repository

↓

git pull

↓

Local Repository

---

# Clone Workflow

GitHub Repository

↓

git clone

↓

Local Computer