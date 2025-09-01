# 📄 Day 06: Searching with `grep` and `find`

## Tasks Completed

-   Practiced searching **inside files** using `grep`

-   Used `grep` flags: `-w`, `-n`, `-i`, `-v` for refined filtering

-   Explored **file-level search** using `find`

-   Combined `find` with `wc -l` using command substitution

-   Learned how shell expansion affects wildcard behavior

-   Compared text-based search with structured data limitations

## Commands Practiced:

```         
# Search for lines containing a pattern
grep "not" haiku.txt                          # Find lines with 'not'
grep "day" haiku.txt                          # Matches 'day', 'today', 'daytime'

# Refine grep matches
grep -w "day" haiku.txt                       # Match whole word 'day' only
grep -n "it" haiku.txt                        # Show line numbers for matches
grep -i "day" haiku.txt                       # Case-insensitive match
grep -v "day" haiku.txt                       # Show lines that do NOT contain 'day'
grep -inw "day" haiku.txt                     # Combine flags: case-insensitive, numbered, whole word

# View grep manual
man grep                                      # Show grep documentation

# Find files and directories
find . -type d                                # List all directories recursively
find . -type f                                # List all files recursively
find . -maxdepth 1                            # Limit search to current directory
find . -mindepth 2                            # Search only 2+ levels deep
find . -empty                                 # Find empty files and directories
find . -perm -u=x -type f                     # Find executable files for user

# Match by name (with quotes to prevent shell expansion)
find . -name '*.txt'                          # Find all .txt files recursively

# Combine find with wc using command substitution
wc -l `find . -name '*.txt'`                  # Count lines in all .txt files found by find

# Combine find + grep
find . -name '*.pdb' | xargs grep "Fe"        # Search for 'Fe' in all .pdb files
```

## Notes:

-   `grep` searches **inside files**, line by line

-   `find` locates **files and directories**, recursively

-   Use single quotes (`'*.txt'`) to prevent shell from expanding wildcards too early

-   Backticks `` `command` `` or `$(command)` allow command substitution

-   `grep` supports regular expressions for advanced pattern matching

-   For non-text data (images, spreadsheets), convert to text or use a programming language like Python

-   Shell tools are powerful but have limits, knowing when to switch to code is part of CLI fluency