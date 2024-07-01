# We will now work on branches 
we will create two branches and work on them how to add files from one branch to other  

- First we need to create new branch- first-branch:
```
git branch first-branch
```
New branch is  created.

- To check list of branch:
```
git branch
```
We will see list of branches. 

- Now get into new branch:
```
git checkout first-branch
```
You will get into new branch.

- Now we will create some files in folder where we opened GIT BASH   
file1 file2 file3

- Now Enter git bash and get list of files, add and commit any one file we are doing in new branch:
```
ls
```
```
git add file1
```
```
git commit -m "commit file1"
```

- Now you will see all files when you see list but when you checkout to other branch there you can only see file2 file3 because there you didn't add , commit file1.
```
git checkout main
```
```
ls
```

# We have command to merge this into other branch if need:
```
git merge first-branch
```
To this you need to be in the branch where you want. For expample you need file1 from first-branch to main, for that you need to be in main and run git merge.
