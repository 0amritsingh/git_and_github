# Advance Tracking and Managing
> Some time we make changes in file and stage the file but then we do some more changes after staging it once then when we do git status we can see that it says you staged this file as well as you have done another change which is not staged yet.

To view Changes: 
1. View unstaged changes
```bash
git diff
```
2. View staged changes
```bash
git diff --staged
```
3. Undo changes in you file
```bash
# this will restore only one file
git restore filename.extention

# this will restore all files
git restore .
```
4. Unstage files
```bash
git restore --staged filename.extention
```
5. Amend a commit 

This allow to make changes in file in a previous commit without creating a new commit
```bash
# Stage the forgotten file
git add forgotten.exstention
 
# Amend the previous commit
git commit --amend -m "New commit message"
```
6. Reset to a Previous Commit
```bash
# Soft Reset (keeps changes in staging):
git reset --soft HEAD~1

# Mixed Reset (keeps changes in working directory):
git reset HEAD~1

# Hard Reset (discards all changes):
git reset --hard HEAD~1
```
Warning: --hard permanently deletes uncommitted work!