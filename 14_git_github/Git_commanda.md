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