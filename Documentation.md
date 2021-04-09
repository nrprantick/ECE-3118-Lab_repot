# Documentation about some git command

## Create a Repository for a Blank (New) Project:

To create a new local repository and apply version control we use: 
```
$ git init
```

## Make copy of existing repository: 
To make a local copy of a remote repository we use: 
```
$ git clone <repository URL>  
```
Usually, the original repository is located on a remote server, often from a Git service like GitHub, Bitbucket, or GitLab. The remote repository URL is referred to the origin.

## Add files to stating area: 
We can add single or multiple files at once in the staging area.To add single file, we use: 
```
$ git add <File name>
```
To add all unstaged files to staging area, we use:
```
$ git add -A
```
## Display the state of the repository and staging area:
 To check the status, we use: 
 ```
 $ git status  
 ```
 The git status command is used to display the state of the repository and staging area. It allows us to see the tracked, untracked files and changes. This command will not show any commit records or information.
 ## Record the changes in the repository:
 When we add a file in Git, it will take place in the staging area. A commit command is used to fetch updates from the staging area to the repository.It is written as: 
 ```
 $ git commit -m "<Commit message>"
 ```
 Here -m is used to display commit messege.The commit command will commit the changes and generate a commit-id. The commit command without any argument will open the default text editor and ask for the commit message. 

 