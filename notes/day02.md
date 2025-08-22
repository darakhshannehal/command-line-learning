## 📄 Day 02: Folder & File Creation

### Tasks Completed:

- Created setup_log.md for validated setup steps.
 
- Created notes/ folder and initialized day01.md and day02.md for daily tracking.
  
- Logged Day 01 and Day 02 setup checkpoints in setup_log.md.

- Documented daily reflections and practiced commands in notes/ using Positron terminal.
  
- Pushed commit to GitHub.

### Commands Practiced:

```
cd ~/Documents/command-line-learning # Navigate to the local project directory

# Create a markdown file for setup steps
touch setup_log.md

# Create a folder for daily notes (with -p to ensure parent folders are created if missing)
mkdir -p notes

# Initialize Day 01 and Day 02 note files inside the notes folder
touch notes/day01.md
touch notes/day02.md

# Stage all changes (new files and folders) for commit
git add .

# Commit with a clear message describing the additions
git commit -m "Add setup_log and notes for Day 01 & 02"

# Push the commit to the GitHub remote
git push -u origin main
```
