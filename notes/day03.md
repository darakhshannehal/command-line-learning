
## 📄 Day 3: File & Directory Operations

## Tasks Completed:

- Created a new directory demo and verified its structure  
- Used nano to create and edit a file (hello) inside demo  
- Practiced file size inspection with ls -s and ls -s -h  
- Deleted files and handled directory removal errors using rm and rmdir  
- Renamed and moved files across directories using mv  
- Copied files within and across directories using cp  
- Validated file existence and structure using ls, ls -a, and pwd

## Commands Practiced:

```
- mkdir demo                 # Create a new directory
- cd demo                   # Move into the new directory
- nano hello                 # Create and edit a text file using Nano
- ls                        # List contents of current directory
- ls -a                     # Show hidden entries (e.g. . and ..)
- ls -s                     # Show file sizes in disk blocks
- ls -sh                    # Show human-readable file sizes
- rm hello                   # Delete file (no undo!)
- cd ..                     # Move up one directory
- rm demo                   # Fails: can't remove non-empty directory
- mv hello greeting   # Rename file (or directory)
- mv greeting .           # Move file to current directory
- cp                  # copy

```
## Notes: 
- nano creates plain text files; use Ctrl+O to save, Enter, then Ctrl+X to exit
- rm deletes permanently — no trash bin or undo
- ls -sh is more readable than ls -s
- mv works for both renaming and relocating
- cp duplicates files; destination can be a file or directory
- . refers to current directory, .. to parent directory
