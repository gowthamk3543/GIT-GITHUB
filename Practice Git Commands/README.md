# GIT Installation
Download the latest version of Git and choose the 64/32 bit version. After the file is downloaded, install it in the system. Once installed, select Launch the Git Bash, then click on finish. The Git Bash is now launched.
```
https://git-scm.com/download/win
```

# GIT Commands
- Check the Git version:
```
git --version
```
- For any help, use the following command:
```
git config --help
```

Now we will Create a Local directory and work on git commands and push the created files to remote repository

- Create a local directory using the following command:
```
mkdir test
cd test
```

- The next step is to initialize the directory:
```
git init
```

Go to the folder where "test" is created and create a text document named "demo." Open "demo" and put any content, like "working on GIT commands" Save and close the file.

- Enter the Git bash interface and type in the following command to check the status:
```
git status
```
This shows that there isn't a file committed yet, and there are untracked files. The untracked files can be seen in red.

- For Git to track that file, add command is used. If you know the exact name of the file, you can specify it:
```
git add demo.txt
```
(We will use `git add .` to add all untracked files)
Now the file is ready to commit

- The next step is to commit the file:
```
git commit -m "commit demo text file"
```

- Let's check the status of the file again:
```
git status
```
You'll notice that there are no more commits to be made and working tree is clean.

- To check all the information regarding the commits that were made:
```
git log
```
This displays the commit ID, author's name, and email ID used. You can also find the date and commit message on the screen.

- Now Go to the folder where "test" is created and edit it and put any content, like "First edit" Save and close the file.

- Enter the Git bash interface and type in the following command to check the status:
```
git status
```
This shows that there isn't a file committed yet, and there is modified file. The modified file can be seen in red. Again we need to add and commit.  

Before doing add and commit we have one more command which is helpfull to check what changes are made and we can compare also:
```
git diff
```
This will show what changes are made.

Now we will add and commit the modified text file:
```
git add .
```
```
git commit -m "commit modified file"
```

- Now we need to config username and email so that we can push files to remote repository:
```
git config --global user.name <your github username>
```
```
git config --global user.email <your github email id>
```
To check the username and email id:
```
git config user.name
```
```
git config user.email
```

- Now, let's push the text document Demo on GitHub. Open your GitHub account, and create a new repository. The name of the repository will be "FirstRepo."
(NOTE: YOU NEED TO HAVE GITHUB ACCOUNT)
Then connect the local repo to remote repo
```
git remote add origin <your github repo URL>
```
Then push the file to remote repo
```
git push -u origin master
```

Now File will be add to Remote repo.

# This is how we transfer files from LOCAL REPO to REMOTE REPO.
