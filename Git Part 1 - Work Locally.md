# Working Locally With Git:

## Creating a brand new git repository

**cd  PROJECT_DIR**

**git config --global user.name "YOUR_NAME"**

**git config --global user.email "YOUR_EMAIL"**

**git init** - Create a brand new Git repository in this directory



## Working with git

**git add .** - Add all changed files

**git add FILENAME** - Add FILENAME again

**git rm --cached FILENAME** - to un-track FILENAME

**git status** - What files have been changed and hints on what to do

**git status -s** - Show what has been changed in compact list

**git commit -m "My First Commit"**

**git commit -a -m "some msg"** - Add files and commit in one command

**git log** - To see all your commits

**git log --pretty=oneline** - See the changes in one compact line

**git log --oneline** - For compact list of commits

**git checkout SHA_NUMBER** - go to previous version of tghe file



## Diff

**git diff** - To see the changes on your files since last commit



## Checkout

**git log --pretty=oneline**
```
b900c412b20d0ae61e4f81f3ec60766bce8f107a file1.txt: Add line 3
2f52aa202095e16a660a5c479524622f6e3c36d2 file1.txt: Add line 2
3c2df3030561f5a49defb108441a7dd850ac1857 Adding file1.txt
```

**git checkout 2f52aa202095e16a660a5c479524622f6e3c36d2**

**git log --pretty=oneline**
```
2f52aa202095e16a660a5c479524622f6e3c36d2 file1.txt: Add line 2
3c2df3030561f5a49defb108441a7dd850ac1857 Adding file1.txt
```

**git checkout master** - return to the master branch

**git log --pretty=oneline**
```
b900c412b20d0ae61e4f81f3ec60766bce8f107a file1.txt: Add line 3
2f52aa202095e16a660a5c479524622f6e3c36d2 file1.txt: Add line 2
3c2df3030561f5a49defb108441a7dd850ac1857 Adding file1.txt
```


##Branches

**git branch** - show all brances

**git branch proj_v2** - create a new brand called proj_v2

**git checkout proj_v2** - working with the new branch

**git add file1.txt**

**git commit -m "commit in the new branch"**

**git checkout master** - Go to the master branch - without line 5

**git merge proj_v2** - Merge file1.txt  from proj_v2 branch

**git branch -d proj_v2** - deleting branch


