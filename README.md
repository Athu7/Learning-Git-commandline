# Learning-Git-commandline
This is a repository created to learn the basics of git command line
## Set username and email
```
git config --global user.name atharva
git config --global user.email atharva.inamdar511@gmail.com
```

## Check the email and username
```
git config --global user.name
git config --global user.email
```

## Check status of your files
```
git status
```

## Move current files to staging are 
```
git add 
```

## Commiting the staged files 
```
git commit
```
write a commit message using VIM editor
To skip the vim editor stage we can write 
```
git commit -m "Commit message"
 ```

## Add all the untracked files to staging area 
```
git add -a
```
When you modify a file in staging area it moves to the modified area
Now we have two versions of the file one is in staging which is before modification and second is the modified version in the modified area.

## Undo the changes made to a file
```
git checkout "filename"
```
This command just matches our file with the last commit.

## Undo the changes made in all the files 
```
git checkout -f
```
Checkout matches your working directory with previously commited files.
## Check all the commits and their details 
```
git log
```
It gives us info about all the commits (author, commit message, data and time)

## Check the most recent commmits
```
git log -p "No. of commits to show"
eg. git log -p 4 to see the 4 recent commits
```

## Check difference between working directory/modified file and staging area
```
git diff 
```

## Check changes between staging area and last commit
```
git diff --staged
```
## Skip the staging area to directly commit files
```
git commit -a -m
```
## Remove file from everywhere
```
git rm "filename"
```
## Remove a folder containing files
```
git rm -r "folder_name"
```

## Remove file from staging area
```
git rm --cached "filename"
```
## Get the summarized status 
```
git status -s
```

## To stop git from tracking certain files
```
touch .gitignore #Creates a gitignore file
```
Now to stop tracking files anywhere in the repo
```
insert "filename" in .gitignore file
```
Stop tracking files with extension ".log"
```
insert  *.log in gitignore file
``` 
Stop tracking the file only in root directory 
```
insert \"filename" in gitignore file
```
Stop tracking a folder/directory
```
insert "foldername"/ in gitignore file
```
 ***

 ## Create a branch in your repo
 ```
 git branch "branch_name"
 ```

 ## Check the current branch
 ```
 git branch
 ```
 Current branch will be shown in green color

 ##  To change the branch 
 ```
 git checkout "branch_name"
```
## Merge a branch into master branch 
First change to a directory you want to merge with
```
git merge "branch_name"
```
## Create a branch and enter into it simultaneously
```
git checkout -b "branch_name"
```
