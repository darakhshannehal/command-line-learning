------------------------------------------------------------------------

## 📄 `notes/day01.md`

## Day 01: Initial Setup

## Tasks Completed:

-   Created GitHub repo with `README.md`
-   Scaffolded local folder structure
-   Created `.gitignore` manually via Notepad
-   Initialized Git and configured identity (per repo)
-   Verified setup and committed `.gitignore`
-   Renamed branch to `main` and linked remote
-   Pulled remote README to resolve mismatch
-   Pushed initial commit to GitHub

## Commands Practiced:

```         

pwd
cd ~/Documents
cd command-line-learning
git init
git config user.name "Your Name Here"
git config user.email "your@email.com"
git config --list
ls -a
git add .gitignore
git commit -m "Add .gitignore"
git branch -m master main
git remote add origin https://github.com/darakhshannehal/command-line-learning
git pull origin main --allow-unrelated-histories
git push -u origin main
```