# Git Fundamentals – Practice Repository

Hands-on practice of Git fundamentals: `add`, `commit`, `checkout`, `reset`, `revert`, `amend`.

> This repository is intentionally simple. The goal is to demonstrate correct Git workflows and a clean commit history.

---

## ✅ What This Repo Demonstrates

- Repository initialization (`git init`)
- Staging and committing (`git add`, `git commit`)
- Modifying tracked files and committing changes
- Discarding local changes (`git checkout -- file`)
- Unstaging changes (`git reset file`)
- Reverting commits safely (`git revert`)
- Rewriting local history (`git reset --hard`)
- Amending the last commit (`git commit --amend`)

---

## 🧠 Tasks + Visual Evidence

> Screenshots are located in `/screenshots`. Each section below includes a visual proof of the exact terminal commands and outcomes.

---

### Task 1 — Git Installation & Configuration
**What I did:** Verified Git installation and configured global username/email.

**Commands:**
- `git --version`
- `git config --global user.name "..."`
- `git config --global user.email "..."`
- `git config --global --list`

**Evidence:**
![Task 1](screenshots/task_1.png)

---

### Task 2 — Create Project Structure
**What I did:** Created two folders and added multiple files into each.

**Commands:**
- `mkdir folderA folderB`
- file creation commands
- `dir`

**Evidence:**
![Task 2](screenshots/task_2.png)

---

### Task 3 — Initialize Git Repository
**What I did:** Initialized the project directory as a Git repository.

**Commands:**
- `git init`

**Evidence:**
![Task 3](screenshots/task_3.png)

---

### Task 4 — Add Files to Staging Area
**What I did:** Added both subfolders to the index (staging area).

**Commands:**
- `git add folderA folderB`
- `git status`

**Evidence:**
![Task 4](screenshots/task_4.png)

---

### Task 5 — Create Initial Commit
**What I did:** Created the first commit from the staged files and verified commit history.

**Commands:**
- `git commit -m "..." `
- `git log --oneline`

**Evidence:**
![Task 5](screenshots/task_5.png)

---

### Task 6 — Modify a File and Commit
**What I did:** Modified a tracked file, staged it, and committed the change.

**Commands:**
- file edit
- `git status`
- `git add ...`
- `git commit -m "..."`
- `git log --oneline`

**Evidence:**
![Task 6](screenshots/task_6.png)

---

### Task 7 — Add a New Folder and Commit
**What I did:** Created a new folder (`folderC`), added files, and committed the folder.

**Commands:**
- `mkdir folderC`
- file creation
- `git add folderC`
- `git commit -m "..."`
- `git log --oneline`

**Evidence:**
![Task 7](screenshots/task_7.png)

---

### Task 8 — Discard Local Changes (No Commit)
**What I did:** Modified a file without committing and discarded the change using checkout.

**Commands:**
- file edit
- `git status`
- `git checkout -- file`
- `git status`

**Evidence:**
![Task 8](screenshots/task_8.png)

---

### Task 9 — Unstage Changes (No Commit)
**What I did:** Staged a modified file, then removed it from the staging area using reset.

**Commands:**
- file edit
- `git add file`
- `git status`
- `git reset file`
- `git status`

**Evidence:**
![Task 9](screenshots/task_9.png)

---

### Task 10 — Revert the Last Commit
**What I did:** Created a commit, then reverted it with `git revert` (history preserved via a new commit).

**Commands:**
- `git commit -m "..."`
- `git revert HEAD`
- `git log --oneline`

**Evidence:**
![Task 10](screenshots/task_10.png)

---

### Task 11 — Hard Reset (Rewrite Local History)
**What I did:** Removed the last commits using a hard reset and verified history changed.

**Commands:**
- `git log --oneline`
- `git reset --hard HEAD~2`
- `git log --oneline`

**Evidence:**
![Task 11](screenshots/task_11.png)

---

### Task 12 — Amend the Last Commit
**What I did:** Amended the most recent commit message without creating a new commit.

**Commands:**
- `git commit --amend -m "..."`
- `git log --oneline`

**Evidence:**
![Task 12](screenshots/task_12.png)

---

## 📌 Repo Structure

