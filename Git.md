# How-To Github

## Creating new project:
$ cd My-Repository
$ git init                    
$ git add README.md			
$ git add .                  
$ git commit -m "First Commit"
$ git remote add origin https://github.com/ilsh1964/My-Repository.git                                       -------- ---------
$ git push -u origin master


## Deleting files on github:
$ git add . -A 
$ git commit -m "removed some files"
$ git push origin master


## Updating git with updated files:
$ git add My_Changed_File
$ git commit -m "My commit explanation"
$ git push


## Get changes FROM GitHub (These commands will bring all the new stuff from GitHub to your machine):
$ git checkout
$ git pull


## Cloning github project to your local machine: 
Copy github repo address (find it in GitHub repo page: git@github.com……/….git)
$ cd Dropbox/Git dir
$ git clone git@github.com……/….git

               
## GENERAL GITHUB REAMRKS:
### We recommend every repository include README, LICENSE, and .gitignore
### Push an existing repository from the command line:
$ git remote add origin https://github.com/ilsh1964/EXAMPLE_FILE.git
$ git push -u origin master




