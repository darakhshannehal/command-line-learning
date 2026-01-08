### Rebase All Commits

1.  Set Notepad as your Git editor (for easier editing)

```         
git config --global core.editor notepad
```

2.  Start the interactive rebase from the very first commit

```         
git rebase -i --root
```

--- IN THE **NOTEPAD WINDOW** THAT OPENS ---

1.  Keep the top (first) commit as 'pick'.

2.  Change all other 'pick' words to 'squash' (or just 's').

TIP: In Notepad, press **Ctrl+H** (Find/Replace).

Replace 'pick ' with 's ' (include the space).

3.  Save and close Notepad.

--- IN THE **SECOND NOTEPAD WINDOW** (Commit Message) ---

Delete the old messages.

Type your new single commit message (e.g., "Initial commit").

Save and close Notepad.

3.  (Optional) If the rebase pauses due to a conflict or manual step:

```         
git rebase --continue
```

4.  Verify that only one commit exists

```         
git log --oneline
```

5.  Force push the clean history to GitHub/Remote

**WARNING**: This overwrites remote history. Use with caution.

```         
git push origin main --force
```

**Outcome**

Your repository now has a single clean commit ("Initial commit"). When you make it public, only this commit will be visible