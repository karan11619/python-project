# Git & GitHub Assessment


# Question 1: Project Initialization & First Push

## Objective
Set up a new Git project and push it to a remote repository.

## Steps Performed

### 1. Create Project Folder
```bash
mkdir python-project
cd python-project
```

### 2. Initialize Git Repository
```bash
git init
```

### 3. Create app.py
```python
print("Hello Git")
```

### 4. Check Git Status
```bash
git status
```

### 5. Stage File
```bash
git add app.py
```

### 6. Commit Changes
```bash
git commit -m "Initial commit with app.py"
```

### 7. Add Remote Repository
```bash
git remote add origin https://github.com/karan11619/python-project.git
```

### 8. Verify Remote
```bash
git remote -v
```

### 9. Push Code
```bash
git branch -M main
git push -u origin main
```

---

# Question 2: Working with Changes & History

## Objective
Track code changes and manage commit history properly.

## Updated app.py

```python
print("Hello Git")

def greet(name):
    print(f"Hello {name}")

greet("Prabakaran")
```

## Check Changes
```bash
git status
```

## View Differences
```bash
git diff
```

## Stage Specific Changes
```bash
git add -p
```

## Commit Changes
```bash
git commit -m "Added greeting function"
```

## Add Another Feature

```python
def add(a, b):
    return a + b

print(add(5, 3))
```

## Stage All Changes
```bash
git add .
```

## Commit Again
```bash
git commit -m "Added add function"
```

## View Commit History
```bash
git log
```

## Compact Commit History
```bash
git log --oneline
```

---

# Question 3: Branching & Feature Development

## Objective
Work with branches and manage feature development.

## Create Feature Branch
```bash
git branch feature-update
```

## Switch Branch
```bash
git checkout feature-update
```

## Add New Feature

```python
def multiply(a, b):
    return a * b

print(multiply(4, 5))
```

## Commit Feature
```bash
git add .
git commit -m "Added multiply feature"
```

## Switch Back to Main
```bash
git checkout main
```

## Merge Feature Branch
```bash
git merge feature-update
```

## Verify Merge
```bash
git log --oneline
```

## Delete Branch
```bash
git branch -d feature-update
```

## Force Delete Dummy Branch
```bash
git checkout -b dummy-branch
git checkout main
git branch -D dummy-branch
```

---

# Question 4: Handling Errors (Stash, Reset, Revert)

## Objective
Learn how to manage mistakes and unfinished work.

## Create Temporary Changes

```python
print("Temporary code")
```

## Stash Changes Including Untracked Files
```bash
git stash -u
```

## Verify Stash
```bash
git stash list
```

## Apply Stashed Changes
```bash
git stash apply
```

## Commit Changes
```bash
git add .
git commit -m "Added temporary code"
```

## Add Incorrect Code

```python
print(10 / 0)
```

## Commit Incorrect Code
```bash
git add .
git commit -m "Added buggy code"
```

## Undo Last Commit Using Reset
```bash
git reset --soft HEAD~1
```

## Add Corrected Code

```python
print("Corrected code")
```

## Commit Corrected Code
```bash
git add .
git commit -m "Added corrected code"
```

## Undo Commit Using Revert
```bash
git revert HEAD
```

## Verify Final History
```bash
git log --oneline
```

---

# Git Commands Used

| Command | Description |
|---|---|
| git init | Initialize repository |
| git status | Check repository status |
| git add | Stage files |
| git commit | Save changes |
| git log | View commit history |
| git branch | Manage branches |
| git checkout | Switch branches |
| git merge | Merge branches |
| git stash | Temporarily save changes |
| git reset | Undo commits |
| git revert | Reverse commits safely |
| git push | Push code to remote repository |

---
