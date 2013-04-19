# How-To Github

## Creating new project
    $ Create a new repository in github.com and paste it's instruction:
    $ cd My-NEW-Repository
    $ git init                    
    $ git add README.md or git add .                  
    $ git commit -m "First Commit"
    $ git remote add origin https://github.com/ilsh1964/My-NEW-Repository.git
    $ git push -u origin master 


## Deleting files on github
    $ git add . -A 
    $ git commit -m "removed some files"
    $ git push origin master


## Updating git with updated files
    $ git add My_Changed_File  or git add .
    $ git commit -m "My commit explanation"
    $ git push


## Get changes FROM GitHub to your machine
    $ git checkout
    $ git pull


## Tags and Diff
    $ cd project_dir
    $ git tag                              \* To show all tags
    $ git tag -a v1.01 -m 'version 1.01'   \* To add new tag 
    $ git tag -l v1.0*                     \* Search tags via wildcard
    $ git show v1.01 
    $ git diff v1.0 v1.01 
    $ git push --tags                      \* To push tags to github.com


## Cloning github project to your local machine
    $ cd Dropbox/Git dir
    $ git clone git@github.com……/….git

               
## REAMRKS
Every repository should include README.md, LICENSE.md, and .gitignore




