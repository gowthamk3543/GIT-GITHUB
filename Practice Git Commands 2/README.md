# Now we will try to pull files from REMOTE REPO to LOCAL REPO
For example we have files in REMOTE repo to get it in LOCAL repo  
We can do it by  
- **git fetch**: Downloads changes from a remote repository but does not merge them into the local branch.
- **git pull**: Downloads changes from a remote repository and immediately attempts to merge them into the current branch.

- We will see Fetch first which is used most of the times:
```
git fetch origin
```

- We use below command to see changes:
```
git diff origin/master
```
This will help us to see the difference and we can merge if we need it. So, we use`git fetch`, `git diff`.

- we will see pull command now which is not used more:
```
git pull origin
```
This will pull files if any changes are made it will also update in local as soon as you pull it. 

# I have uploaded Document you can refer it.
