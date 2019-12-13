# How to GIT ??
## Personnal memento of main commands & functions
###### By J-Pard, thanks to BeCode.

 ## 1. General Schedule :  
-------------

1. Connect to Github and copy the clone-URL of wanted repository.
2. Clone the repo in your local folder.
      > git clone url
3. Access the folder and check existing features (branches, files, ...).
      > cd repositoryName  
      > ls  
      > git branch -a
4. Create a new branch and move into it.
      > git branch branchName  
      > git checkout branchName
5. Verify the version of the file.
      > git pull origin branchToCheck
6. Modify the file with :
      > nano file.name  
      > external editor
7. Prepare the file for *staging*.
      > git add file.name
8. Check if file is clean & ready :
      > git status
9. Confirm modification and commit it.
      > git commit -m "What you have done and why ?"
10. Now, you can send your file(s) to the distant repository (alias *remote* ):
      > git push origin branchToPush

11. If work is **WORKING AND VALIDATED**, you can *merge* it on the principal branch.
/!\ Avoid as possible to merge on *master* branch /!\
      > git checkout confirmedBranch
      > git push origin confirmedBranch  

 ## 2. Basics commands :  
-------------

| Commands                   | Actions                                             |
| -------------------------- | --------------------------------------------------- |
| git init                   | Initialise the git local folder                     |
| git clone url              | Clone a repo into local folder                      |
| git branch                 | Show accessibles branches                           |
| git branch -a              | Show all existing tables and active position        |
| git branch branchName      | Create a branch as branchName                       |
| git checkout branchName    | Move to branchName                                  |
| git checkout -b branchName | Create and move to new branchName                   |
| git branch -d branchName   | Delete the branch branchName (only if empty)        |
| git branch -D branchName   | Delete the branch branchName even if it's not empty |
| git status                 | Show actual status of actives files                 |
| git add file.name          | Prepare file to staging                             |
| git commit -m " "          | Commit prepared file(s) + "What and why"            |
| git commit -am " "         | Prepare & Commit file(s) already in index           |
| git push origin branch     | Send file(s) to Github repository                   |
| git pull origin branch     | Download file from origin branch                    |
| git merge branchToMerge    | Merge branch to current branch location             |
