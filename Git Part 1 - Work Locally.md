# Working Locally With Git:

### Creating a brand new git repository

** cd  PROJECT_DIR **

** git config --global user.name "YOUR_NAME" **

** git config --global user.email "YOUR_EMAIL" **

** git init ** Creating a brand new Git repository in this directory


### Worging with git

* git status * What files have changed/not tracked and hints on what to do

* git add . * Add all changed files

* git rm --cached FILENAME * to un-track FILENAME

* git add FILENAME * Add FILENAME again

* git commit -m "My First Commit"

* git log* To see your commits

* git log --pretty=oneline * See the changes in one compact line

* git checkout SHA_NUMBER 


### Modify\Change your files
**git statusi** You'll notify that the file was updated and you need to commit the changes

**git diff (To see the changes on your files since last commit)

**git diff --cached

**git add .

**git commit -m "My Second Commit"

**git logi** If the log is too large: hold shift + zz  to exit)


Checkout: suppose you have this situation
git log --pretty=oneline
b900c412b20d0ae61e4f81f3ec60766bce8f107a file1.txt: Add line 3
2f52aa202095e16a660a5c479524622f6e3c36d2 file1.txt: Add line 2
3c2df3030561f5a49defb108441a7dd850ac1857 Adding file1.txt


git checkout 2f52aa202095e16a660a5c479524622f6e3c36d2    (go to previous version of file1)
git log --pretty=oneline
2f52aa202095e16a660a5c479524622f6e3c36d2 file1.txt: Add line 2
3c2df3030561f5a49defb108441a7dd850ac1857 Adding file1.txt


git checkout master (go back to the updated situation)
git log --pretty=oneline
b900c412b20d0ae61e4f81f3ec60766bce8f107a file1.txt: Add line 3
2f52aa202095e16a660a5c479524622f6e3c36d2 file1.txt: Add line 2
3c2df3030561f5a49defb108441a7dd850ac1857 Adding file1.txt


branch:
git branch (show your brances)
git branch proj_v2 (create a new brand called proj_v2)
git checkout proj_v2 (working with the new branch)
git add file1.txt
git commit -m "commit in the new branch"

git checkout master (go to the master branch - without line 5)
git merge proj_v2 (merge file1.txt  from proj_v2 branch)
git branch -d proj_v2 (deleting branch)


Usefull commands:
git log --oneline (to see compact list of commits, only with it's commit text msg)
git commit -a -m "some msg" (add files and commit in one command)
gt status -s (show what has changed in compact list)    

+------------+          +------------+           +------------------+         +-------------------+
|            |--add---> |INDEX CACHE |--commit-> | Local Repository +--push-->| Remote Repository |
| Working Dir|          +------------+           +----------v---^---+-<-pull--+-------------------+                   
|            |<-----------checkout HEAD---------------------+   |pull                |
|------------+<------------------pull---------------------------^--------------------|
                                                                                   
                                                                                    
