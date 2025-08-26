## 📄 Day 04: Pipes, Filters, and Special Characters

## Tasks Completed:
- Created 8 dummy FASTA files with headers and DNA sequences.
- Used wc to inspect file content and redirected output to a file.
- Sorted line counts and extracted shortest file using sort and head.
- Combined commands with pipes (|) to streamline workflows.
- Practiced filters: tail, cut, uniq, split.
- Applied wildcards (*, ?) and input/output redirection (<, >).

## Commands Practiced:

```
Create dummy FASTA files
- echo -e ">seq1\nATGCGTACGTAGCTAG" > sample1.fasta
- Repeated for sample2.fasta to sample8.fasta

Count lines, words, characters
- wc *.fasta                                      # Full count per file
- wc -l *.fasta                                   # Line count only
- wc -l *.fasta > lengths                         # Redirect output to file
- ls lengths                                      # Confirm file creation
- cat lengths                                     # View contents of lengths

Sort and extract shortest file
- sort lengths > sorted-lengths                   # Sort line counts
- head -1 sorted-lengths                          # View first line
- sort lengths | head -1                          # Pipe without intermediate file
- wc -l *.fasta | sort | head -1                  # Full pipeline

Bonus filters
- tail -n 1 sample*.fasta                         # Show last line (sequence)
- cut -c 1-10 sample*.fasta                       # Extract first 10 characters
- cat sample*.fasta | sort | uniq                 # Remove duplicate lines
- cat sample*.fasta | sort | uniq -c              # Count unique lines
- cat sample*.fasta > all_sequences.fasta         # Combine all files
- split -l 4 all_sequences.fasta chunk_           # Split into chunks

Special characters
- ls sample*.fasta                                # Match all FASTA files
- ls sample?.fasta                                # Match files with single-digit suffix
- sort < sample4.fasta                            # Input redirection

```
## Notes: 
wc shows lines, words, and characters per file
- wc -l → lines only
- wc -w → words only
- wc -c → characters only
  
## Behind the Scenes: Processes and Streams
Each command runs as a process. It has:
- Standard input (**stdin**) → where it reads from
- Standard output (**stdout**) → where it writes to
- Pipes connect stdout of one process to stdin of the next.
  

