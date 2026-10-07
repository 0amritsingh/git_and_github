# Branches, Merge and Merge conflict
> some info about branches soon

List branches
```bash
git branch
```

Create new branch
```bash
git branch new-branch-name
```

Switch branches
```bash
git switch branch-name
```

Create and switch branches
```bash
git switch -c new-branch-name
```

Delete a branch 
```bash
git branch -d branch-name
```

Merging branches
```bash
# enter in the branch in which you want to merge and then 
git merge branch-name
```

> **Merge Conflict:** Suppose if you're working on a file in branch A and you made a new branch named B you made some changes in the same file in branch A and someone made some other changes in branch B on the same file if you try to merge both the branches you face a conflict because there has been made two different kinds of changes in two different branches.

> **Resolve Conflict:** To reslove confict in the conflicting file you must keep one change from one branch for that you can run the following command to keep code of a spicfic type: 

To keep changes from the current branch:
```bash
git checkout --ours filename.extention
```

To keep changes from the previous branch:
```bash
git chechout --theirs filename.extention
```