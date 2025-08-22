# Git Setup Log

This file documents reproducible Git setup steps for the `command-line-learning` project.

## Day 01: Initial Setup

### Create GitHub Repo

-   Repo name: `command-line-learning`
-   Add `README.md` directly on GitHub

### Local Folder Setup

-   Create folder `command-line-learning` in `Documents`

### Create `.gitignore`

-   Open Notepad and manually add standard `.gitignore` entries
-   Save as `.gitignore` and move into local folder

### Git Bash Navigation
```         
pwd # Confirm current working directory

cd ~/Documents

cd command-line-learning
```

### Initialize Git and set local identity (important on shared devices)

```         
git init

git config user.name "Your Name Here"

git config user.email "your\@email.com"
```

### Verify identity setup

```         
git config --list # Press 'q' to exit pager if needed
```

### Confirm .gitignore presence and commit it

```         
ls -a # Validate that .gitignore is present
git add .gitignore 
git commit -m "Add .gitignore"
```

### Rename local branch to match GitHub default

```         
git branch -m master main
```

### Connect to GitHub repo

```         
git remote add origin https://github.com/darakhshannehal/command-line-learning
```

### Pull remote README.md to resolve mismatch

```         
git pull origin main --allow-unrelated-histories # to merge local repo with GitHub’s README
```

### Push local changes to GitHub

```         
git push -u origin main
```

------------------------------------------------------------------------


## Day 02

- Created `setup_log.md` and `notes/` folder; initialized `day01.md` and `day02.md` for daily tracking.
- Logged setup steps in `setup_log.md`, and documented daily notes in `notes/` using **Positron terminal**

