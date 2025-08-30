# 📄 Day 05: File Permissions

## Tasks Completed:
- Learned how Unix manages file access using users, groups, and permission categories
- Interpreted permission strings using ls -l and ls -a -l
- Explored the meaning of x for directories (traversal vs execution)
- Modified file permissions using chmod
- Created a simple executable script using cat > filename and chmod u+x
- Compared Unix permissions with Windows ACLs

## Commands Practiced:
```
# View file permissions and metadata
- ls -l                      # Long-form listing with permissions, owner, group, size, timestamp
- ls -a -l                   # Includes hidden entries like . and ..

# Change file permissions
- **chmod** u=rw grades.txt      # Give user read/write, remove execute
- chmod g=r grades.txt       # Give group read-only
- chmod a= grades.txt        # Remove all permissions for others
- chmod u+x smallest         # Add execute permission for user

# Create a script interactively
- cat > smallest             # Start writing to a file named 'smallest'

# Type the following line, then press Ctrl+D to save and exit:
- wc -l *.pdb | sort | head -1

# Run the script
./smallest                 # Execute the script from current directory

```

## Notes:
- Unix tracks permissions for three categories: owner, group, and others
- Permission triplets: **r** (read), **w** (write), **x** (execute); - means permission is off
- x on directories means traversal, not execution
- chmod modifies permissions: u (user), g (group), a (all); use +, -, or = to adjust
- cat > filename lets you write directly into a file from the terminal
- Ctrl+D ends input when using cat interactively
- ./filename ensures you run the script in your current directory, not a system-wide one
- Windows uses **ACLs** (Access Control Lists), which are more flexible but harder to manage
