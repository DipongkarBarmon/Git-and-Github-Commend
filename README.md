 # Git and Github command

Learn about Git and Github topic

1. Git and Github basic 

2. Basic command of Git

3. PR marging, Branching stratagies for Devops

4. Hooks (pre-commit Hooks)

5. Repo setup end to end (GitHub Actions CI/CD)



gitlab = github = bitbucket 


differece between file system and version control system

git = version control system

in file system we can not track the changes of the file and can't recover delete file

git is a version control system which is used to track the changes of the file and can recover delete file

to convert file system to version control system we need to initialize the git repository

# Command of Git

***git status = check the status of the file . we can use any time after git init


****git init = initialize empty the git repository 

 

# git add command : to add the file to the staging area that means untracked to tracked file

git add <file_name> = add the file to the staging area

****git add . = add all the file to the staging area

git add -A = add all the file to the staging area

before add file they are untracked file

after add file to the staging area we need to commit the file to the local repository

the file which is in the staging area is called as tracked file

# git rm command : to remove the file from the staging area that means tracked to untracked file 

git rm = remove the file from the staging area

git rm --cached = remove the file from the staging area but not from the working directory

git rm --cached <file_name> = remove the file from the staging area but not from the working directory

git rm --cached . = remove all the file from the staging area but not from the working directory

git rm --cached -r <folder_name> = remove the folder from the staging area but not from the working directory

*****git rm --cached -r . = remove all the folder from the staging area but not from the working directory


# git commit command : to commit the file to the local repository that means tracked to committed file

git commit = commit the file to the local repository

****git commit -m "message" = commit the file to the local repository with message

# recovery of delete file


rm <file_name> -> delete the file from the working directory

git rm <file_name> -> delete the file from the staging area and working directory it delete file permanently 


these file are not delete from version control system 

we can recover the file using git checkout command

git checkout -- <file_name> = recover the file from the staging area

****git checkout -- . = recover all the file from the staging area
 
<!-- git checkout -f = recover all the file from the staging area and working directory

git checkout -f <file_name> = recover the file from the staging area and working directory

git checkout -f . = recover all the file from the staging area and working directory  -->

# or 
# restore command 
git restore = recover the file from the staging area

git restore <file_name> = recover the file from the staging area

****git restore . = recover all the file from the staging area




# to push code local to github 

****git remote add origin <url> = add the remote repository

if we want to change the remote repository url then we can use the following command

git remote set-url origin <url> = change the remote repository url

in local repository branch is master and in remote repository branch is main

then we need to change the branch name from master to main
using this command ***git branch -M main = change the branch name from master to main

we can check the branch name using this command ***git branch

****git push -u origin main = push the file to the remote repository

****git remote -v = to check the remote repository url

we also push code without changing branch 
we need to use passKey to push the code to the remote repository
generate passkey from github account settings -> developer settings -> personal access tokens -> generate new token -> copy the token

***git remote set-url http://passkey@<url>

****git push -u origin master = push the file to the remote repository

after any change we just use to push code
git push = push the file to the remote repository