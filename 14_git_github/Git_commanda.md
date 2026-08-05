# Git Commands

This document contains the most commonly used Git commands along with their purpose, syntax, examples, and expected output.

---

# 1. git status

## Purpose

Displays the current status of the Git repository.

It shows:
- Modified files
- New (untracked) files
- Staged files
- Current branch

## Syntax

```bash
git status
```

## Example

```bash
git status
```

## Expected Output

```text
On branch main

Changes not staged for commit:
modified: README.md
```

---

# 2. git add .

## Purpose

Stages all new and modified files for the next commit.

The dot (.) means "all files in the current repository."

## Syntax

```bash
git add .
```

## Example

```bash
git add .
```

## Output

No output is shown if the command is successful.

---

# 3. git commit

## Purpose

Creates a snapshot (checkpoint) of the staged files.

Each commit stores:
- Project state
- Author
- Date
- Commit message

## Syntax

```bash
git commit -m "Commit Message"
```

## Example

```bash
git commit -m "Added Git basics documentation"
```

## Example Output

```text
[main abc1234] Added Git basics documentation
5 files changed
```

---

# 4. git push

## Purpose

Uploads local commits to the remote GitHub repository.

## Syntax

```bash
git push
```

## Example

```bash
git push
```

## Example Output

```text
Enumerating objects...
Writing objects...
Done
```

---

# 5. git pull

## Purpose

Downloads the latest commits from GitHub and updates the local repository.

## Syntax

```bash
git pull
```

## Example

```bash
git pull
```

## Example Output

```text
Already up to date.
```

---

# 6. git log

## Purpose

Displays the complete commit history.

## Syntax

```bash
git log
```

## Example Output

```text
commit ab2747f
Author: Nikhil Reddy

Added Git basics documentation
```

### Exit git log

Press

```text
q
```

to return to the terminal.

---

# 7. git log --oneline

## Purpose

Displays commit history in a short format.

## Syntax

```bash
git log --oneline
```

## Example Output

```text
ab2747f Added Git basics documentation
983e1c9 Initial commit
```

---

# 8. git diff

## Purpose

Shows the difference between the last committed version and the current modified version.

Useful before committing.

## Syntax

```bash
git diff
```

## Example Output

```diff
+ Added one new line
```

### Meaning

+ → Added line

- → Deleted line

---

# 9. git restore

## Purpose

Restores a file to its last committed version.

It removes uncommitted changes.

## Syntax

```bash
git restore filename
```

## Example

```bash
git restore README.md
```

---

# 10. git branch

## Purpose

Displays all branches.

Can also create a new branch.

## Show Branches

```bash
git branch
```

Output

```text
* main
```

The * indicates the current branch.

---

## Create Branch

```bash
git branch practice_branch
```

Output

```text
* main
practice_branch
```

---

# 11. git switch

## Purpose

Switches between branches.

## Syntax

```bash
git switch branch_name
```

## Example

```bash
git switch practice_branch
```

Return to main

```bash
git switch main
```

---

# 12. git remote

## Purpose

Displays the configured remote repository names.

## Syntax

```bash
git remote
```

## Example Output

```text
origin
```

---

# 13. git remote -v

## Purpose

Displays the remote repository URLs.

## Syntax

```bash
git remote -v
```

## Example Output

```text
origin  https://github.com/Nikhilreddy0724/VLSI-Portfolio.git (fetch)

origin  https://github.com/Nikhilreddy0724/VLSI-Portfolio.git (push)
```

---

# 14. git clone

## Purpose

Downloads a repository from GitHub.

Usually used when setting up a project on a new computer.

## Syntax

```bash
git clone repository_url
```

## Example

```bash
git clone https://github.com/Nikhilreddy0724/VLSI-Portfolio.git
```

---

# 15. Git Command Flow

```text
Create File
      │
      ▼
git status
      │
      ▼
git add .
      │
      ▼
git commit -m "message"
      │
      ▼
git push
      │
      ▼
GitHub
```

---

# Daily Git Workflow

1. Create or modify files.
2. Save the files.
3. Check changes using `git status`.
4. Stage the files using `git add .`.
5. Create a commit using `git commit -m "Meaningful message"`.
6. Upload changes using `git push`.
7. Verify the changes on GitHub.

---

# Summary of Commands

| Command | Purpose |
|----------|----------|
| git status | Show repository status |
| git add . | Stage all changes |
| git commit -m "message" | Save a snapshot |
| git push | Upload commits to GitHub |
| git pull | Download latest changes |
| git log | View commit history |
| git log --oneline | View short commit history |
| git diff | Show changes before committing |
| git restore | Discard uncommitted changes |
| git branch | List or create branches |
| git switch | Switch branches |
| git remote | Show remote names |
| git remote -v | Show remote URLs |
| git clone | Download a repository |