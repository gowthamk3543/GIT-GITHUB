# **Git Installation on Windows**

Download the latest version of Git and choose the 64/32 bit version. After the file is downloaded, install it in the system. Once installed, select Launch the Git Bash, then click on finish. The Git Bash is now launched.

```
https://git-scm.com/downloads
```

# **GIT COMMANDS**

To check git version
```
git --version
```

For any help, use the following command
```
git config --help
```

**Now we create local directory, work on git commands and later push it to remote repository**

1) Create a local directory using the following command
```
mkdir test
cd test
```
2) The next step is to initialize the directory:
```
git init
```
3) Go to the folder where "test" is created and create a text document named "demo." Open "demo" and put any content, like "Learning GIT and GITHUB Save and close 
   the file.  
   (NOTE: FOLDER WHERE "test" MEANS YOU SHOULD DO IT IN NOTEPAD)
   
5) Enter the Git bash interface and type in the following command to check the status:
```
git status
```
This shows that there isn't a file committed yet, and there are untracked files. The untracked files can be seen in red.

6) For Git to track that file, add command is used. If you know the exact name of the file, you can specify it:
```
git add demo.text
```
(If we use `git add .` it will add all files which are in untrackked files)  
(If we see status `git status`   you can see that file is ready to commit)

7) The next step is to commit the file.
```
git commit -m "commit demo file"
```

8) Now if we check status
```
git status
```
You'll notice that there are no more commits to be made.

9) To  check all the information regarding the commits that were made
```
git log
```
This displays the commit ID, author's name, and email ID used. You can also find the date and commit message on the screen.  

10) Now edit the same file text document demo

Enter the Git bash interface and type in the following command to check the status:
```
git status
```
we see that file is modified which needs to be added and commited as we did before.  

Before we add and commit we have command which is used to compare what changes have made
```
git diff
```
Now we will add and commit
```
git add .
```
```
git commit -m "commit modified demo file"
```

11) Now we will push this file text document demo on GitHub.
In order to do it we need to config user.name and user.email we do it by
```
git config --global user.name <replace your username>
```
```
git config --global user.email <replace your email id>
```
To check the list of username and email we use
```
git config user.name
```
```
git config user.email
```

12) Open your GitHub account, and create a new repository. The name of the repository will be "FirstRepo."
(NOTE: YOU NEED TO HAVE GITHUB ACCOUNT)

13) Enter Git bash interface and type in the following commands to push the file to remote repository (FirstRepo)
```
git remote add origin <your github repository url>
```
```
git push -u origin master
```

# This is how we push the file from LOCAL REPO to REMOTE REPO
