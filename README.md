### 1) `ls` — list files
- `ls` — list files in the current directory  
- `ls -l` — long listing (permissions, owner, size, date)  
- `ls -la` — include hidden files (those starting with `.`)

---

### 2) `cd` — change directory
- `cd` — go to your home directory  
- `cd path/to/dir` — go to a directory  
- `cd ..` — go up one level  
- `cd -` — jump back to previous directory

---

### 3) `pwd` — print working directory
- `pwd` — show the full path of where you are

---

### 4) `mkdir` — create directories
- `mkdir newdir` — create a directory named `newdir`  
- `mkdir -p a/b/c` — create nested directories if parents don’t exist

---

### 5) `rm` — remove files/directories
- `rm file` — delete a file  
- `rm -r dir` — delete a directory **recursively**  
- `rm -rf dir` — force recursive delete (no prompts) **dangerous — double-check the path**

---

### 6) `cp` — copy files/directories
- `cp src dest` — copy a file  
- `cp -r dir1 dir2` — copy a directory recursively  
- `cp -i src dest` — interactive (asks before overwrite)

---

### 7) `mv` — move/rename files and directories
- `mv old new` — rename  
- `mv file dir/` — move a file into a directory  
- `mv -i src dest` — interactive (asks before overwrite)

---

### 8) `grep` — search text
- `grep "pattern" file` — show lines matching `pattern`  
- `grep -n "pattern" file` — show line numbers  
- `grep -r "pattern" dir/` — search recursively in a directory  
- Common add-ons: `-i` (ignore case), `-v` (invert match)

---

## Git Commands

### 9) `git status` — see what changed
- `git status` — shows branch, staged/unstaged files, untracked files

---

### 10) `git add` — stage changes
- `git add file` — stage a specific file  
- `git add .` — stage everything in the current directory  
- `git restore --staged file` — unstage if you changed your mind

---

### 11) `git commit` — save a snapshot
- `git commit -m "message"` — commit staged changes with a message  
- `git commit -am "message"` — stage **modified tracked** files and commit (doesn’t add new files)  
- Good messages: short summary in present tense (e.g., “Add ls section”)

---

### 12) `git log` — view history
- `git log` — detailed history  
- `git log --oneline` — compact one-line commits  
- `git log --oneline --graph --decorate --all` — nice visual overview

---

### 13) `git branch` — list/create/delete branches
- `git branch` — list local branches  
- `git branch new-branch` — create a branch (stay where you are)  
- `git branch -d branch-name` — delete a **merged** branch  
- `git branch -D branch-name` — force delete (use with care)

---

### 14) `git checkout -b` — create & switch to a branch
- `git checkout -b feature-x` — create branch and switch to it  
- `git checkout main` — switch back to `main`

---

### 15) `git merge` — combine branches
- `git checkout main` — first, be on the branch that will receive changes  
- `git merge feature-x` — merge `feature-x` into `main`  
- If there are conflicts: open the files, keep the correct lines, then  
  - `git add <file>`  
  - `git commit` (completes the merge)

---
