
## 📄 Day 1: Initial Setup

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
- pwd                                   # Print current working directory to confirm location
- cd ~/Documents                        # Navigate to the Documents folder
- cd command-line-learning               # Enter your project directory
- git init                                   # Initialize a new Git repository locally
- git config user.name "Your Name Here"               # Set your Git username for this repo 
- git config user.email "your@email.com"              # Set your Git email for this repo
- git config --list                          # Verify current Git configuration
- ls -a                                      # List all files, including hidden ones like .git and .gitignore
- git add .gitignore                         # Stage the .gitignore file for commit
- git commit -m "Add .gitignore"                    # Commit the staged file with a descriptive message
- git branch -m master main                         # Rename default branch from 'master' to 'main' for consistency with GitHub
- git remote add origin https://github.com/darakhshannehal/command-line-learning        # Link local repo to GitHub remote
- git pull origin main --allow-unrelated-histories                                      # Pull from remote main branch, allowing merge of unrelated histories
- git push -u origin main                                                               # Push local commits to GitHub and set upstream tracking for future syncs

```
