# Connecting to Remotes
View Remotes
```bash
git remote -v
```

Add Remote
```bash
git remote add origin https://github.com/username/repository.git
```

Change Remote URL
```bash
git remote set-url origin https://github.com/username/new-repo.git
```

# Core Operations
Clone Repository
```bash
git clone https://github.com/username/repository.git
```

# Push Changes
```bash
# First push (set upstream)
git push -u origin main
 
# Regular push
git push
 
# Push specific branch
git push origin branch-name
```

# Pull Changes
```bash
# Pull (fetch + merge)
git pull
 
# Pull specific branch
git pull origin branch-name
```

# Fetch Changes
```bash
# Fetch without merging
git fetch
 
# Fetch all remotes
git fetch --all
```

# Branch Management
List Remote Branches
```bash
git branch -r
```

Delete Remote Branch
```bash
git push origin --delete branch-name
```
