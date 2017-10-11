# Working Locally With Git:

## Creating a brand new git repository

**cd  PROJECT_DIR**

**git --version - Print Git version

**git config --global user.name "YOUR_NAME"**

**git config --global user.email "YOUR_EMAIL"**

**git config --global core.editor "vim"** - Change the default editor

**git config --list** - Show your config

**git help** - Bring all git help command

**git help add** - help on add command



## Working with git

**git init** - Create a brand new Git repository in this directory

**git add .** - Add all changed files to stage area

**git add -A** - Add all changed files to stage area

**git add *.txt** - Add all *.txt files to stage area

**git add FILENAME** - Add FILENAME again

**git reset FILENAME** - Remove file from staging area

**git reset ** - Remove all files from staging area

**git rm --cached FILENAME** - to un-track FILENAME (remove from staging area)

**git rm -f FILENAME** - Delete FILENAME from os

**git mv XXX YYY** - Rename filename XXX to YYY

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


##Git Log
```
git log # Shows all of the previous commit messages in reverse order
git log --pretty=oneline # Shows commits on one line
git log --pretty=format:"%h : %an : %ar : %s"
  %h - Abbreviated Hash
  %an - Authors Name
  %ar - Date Changed
  %s - First Line of Comment
git log -p -2 # Shows the last 2 commit changes
git log --stat # Prints abbreviated stats
git log --since=1.weeks # Show only changes in the last week
git log --since="2014-04-12" # Show changes since this date
git log --author="Derek Banas" # Changes made by author
git log --before="2014-04-13" # Changes made before this date

```


##Branch and Merging

**git branch** - show all brances

**git branch proj_v2** - create a new brand called proj_v2

**git checkout proj_v2** - working with the new branch

**git checkout -b proj_v2** - create a new branch and jump to it

**git add file1.txt**

**git commit -m "commit in the new branch"**

**git checkout master** - Go to the master branch - without file1.txt

**git merge proj_v2** - Merge file1.txt from proj_v2 branch

**git branch -d proj_v2** - deleting merge  branch

**git branch -D proj_v2** - deleting dont merge  branch


##.gitignore  (must be in project dir - not in .git)

*.apk

*.exe

.ThisDir

bin/


##Common workflow:
**git branch new_branch_name**
**git branch** see all branches. *master is the activated bransh
**git checkout new_branch_name**start working with the new branch
**git branch** see all branches. *new_branch_name is the activated bransh
**make changes to the source code**
**git add -A**
**git commit -m "message"** it commit the changed to the branch. it's no effect to the master or remote repository
**git push -u origin new_branch_name** push this branch to remote repository
**git merge new_branch_name** merge new_branch_name with master branch
**git push origin master** push this branch to remote repository
**git branch -d new_branch_name** delete not needed branch



## Remarks
*** The stage area allow you all time add several files and commit them (it allow
you nor commit all files al ones)
