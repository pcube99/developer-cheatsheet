# Git cheatsheet

### 1) Turn an existing directory into a git repository 
```
git init
```
### 2) Download or clone a repo
```
git clone [url]
```
### 3) Sets the name you want attached to your commit transactions 
```
git config --global user.name "[name]"
```
### 4) Sets the email you want attached to your commit transactions 
```
git config --global user.email "[email address]"
```
### 5) To create a new branch 
```
git branch "branch-name"
```
### 6) Switch to another branch
```
git checkout "branch-name"
```
### 7) Check which branch is active 
```
git status
```
### 8) Delete a branch 
The -d option stands for --delete, which would delete the local branch, only if you have already pushed and merged it with your remote branches.
```
git branch -d "branch-name"
```
The -D option stands for --delete --force, which deletes the branch regardless of its push and merge status, so be careful using this one!
```
git branch -D "branch-name"
```
### 9) Delete branch in remote repo  
```
git push "remote-name" --delete "branch-name"
```
### 10) Mereg another branch's changes into your current branch 
```
git merge "branch-name"
```
### 11) Uploads all local branch commits to GitHub
```
git push origin
```
### 12) Commit local changes into remote repo
```
git commit -m "commit-message"
```
### 13) Updates your current local working branch with all new commits from the corresponding remote branch
```
git pull
```
### 14) Temporary save your local branch changes
```
git stash
```
### 15) View and fetch your temporary changes from local branch
```
git stash pop
```
### 16) Reset a commit
```
git reset "commit-id"
```
### 17) Updating the local list of remote branches
```
git remote update origin --prune
```
