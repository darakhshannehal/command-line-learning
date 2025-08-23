
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
- cd ~/Documents/command-line-learning   # Navigate to working directory
- ls -F                                  # List contents with indicators
- mkdir demo                             # Create new directory
- ls demo                                # Check contents of demo (empty)
- cd demo                                # Enter demo directory
- nano hello                             # Create and edit file
- ls -s                                  # Show file size in blocks
- ls -s -h                               # Show human-readable file size
- rm hello                               # Delete file
- cd ..                                  # Move up one level
- rm demo                                # Attempt to remove directory (fails)
- rmdir demo                             # Attempt to remove non-empty directory (fails)
- rm demo/hello                          # Delete file inside demo
- rmdir demo                             # Remove now-empty directory
- mv demo/hello demo/greeting            # Rename file inside demo
- mv demo/greeting .                     # Move file to current directory
- cp greeting demo/hello                 # Copy file back into demo
- rm greeting                            # Delete moved file
- cp demo/hello .                        # Copy file again to current directory
- ls                                     # Validate final structure

```
## Notes: 
- ls -F helps distinguish files (README.md) from directories (demo/)
- nano creates plain text files; use Ctrl+O to save, Enter, then Ctrl+X to exit
- rm deletes permanently — no trash bin or undo
- ls -sh is more readable than ls -s
- mv works for both renaming and relocating
- cp duplicates files; destination can be a file or directory
- . refers to current directory, .. to parent directory
