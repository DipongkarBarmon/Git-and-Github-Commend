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

git init = initialize empty the git repository 

git status = check the status of the file

# git add command : to add the file to the staging area that means untracked to tracked file

git add <file_name> = add the file to the staging area

git add . = add all the file to the staging area

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

git rm --cached -r . = remove all the folder from the staging area but not from the working directory



git commit = commit the file to the local repository

git log = check the history of the commit

git diff = check the difference between the file

git checkout = checkout the file

git reset = reset the file

git rm = remove the file

git mv = move the file

git branch = check the branch

git checkout -b = create the branch

git merge = merge the branch

git remote = check the remote repository

git push = push the file to the remote repository

git pull = pull the file from the remote repository

git clone = clone the remote repository

git fetch = fetch the file from the remote repository

git stash = stash the file

git tag = tag the file

git show = show the file

git blame = blame the file

git grep = grep the file

git config = config the file

git help = help the file

git init = initialize empty the git repository

git status = check the status of the file

git add = add the file to the staging area

git commit = commit the file to the local repository

git log = check the history of the commit

git diff =