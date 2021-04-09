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

 ## Check the last commit point: 
 The git show head is used to check the status of the Head. This command will show the location of the Head. Syntax:

```
$ git show HEAD  
```
### Review and read full history:
The basic git log command will display the most recent commits and the status of the head. It will use as:
```
$ git log  
```
## Connect local repository to remote repository: 
To check the configuration of the remote server, run the git remote command. The git remote command allows accessing the connection between remote and local. It can be used as:
```
$ git remote  
```
Git remote supports a specific option -v to show the URLs that Git has stored as a short name. These short names are used during the reading and write operation. Here, -v stands for verbose. It is used as:
```
$ git remote -v  
```
When we fetch a repository implicitly, git adds a remote for the repository. Also, we can explicitly add a remote for a repository. We can add a remote as a shot nickname or short name. To add remote as a short name, follow the below command:
```
$ git remote add <short name><remote URL>  
```
##  Switch between branches in a repository: 
We can perform many operations by git checkout command like the switch to a specific branch, create a new branch, checkout a remote branch, and more. The git branch and git checkout commands can be integrated.

To demonstrate available branches in repository, use the below command:
```
$ git branch  
```
Now, we have the list of available branches. To switch between branches, use the below command.
```
$ git checkout <branchname>  
```
##  Fetch the complete repository: 
We can pull the repository by using the git pull command. The syntax is given below:
```
$ git pull <options><remote>/<branchname>  
```
like,
```
$ git pull origin master  
```
In the above syntax, the term origin stands for the repository location where the remote repository situated. Master is considered as the main branch of the project.

We can fetch the complete repository with the help of fetch command from a repository URL. It is just like pull command.
```
$ git fetch< repository Url>  
```
We can fetch a specific branch from a repository. It will only access the element from a specific branch. Syntax:
```
$ git fetch <branch URL><branch name>  
```
It is recomanded to fetch everytime before start working, when we work on a group. So, we can be updated with team-members.
## Upload files to remote repository:
To upload files we use git push.The push term refers to upload local repository content to a remote repository. Pushing is an act of transfer commits from your local repository to a remote repository. Pushing is capable of overwriting changes; caution should be taken when pushing.
Git push origin master is a special command-line utility that specifies the remote branch and directory. When you have multiple branches and directory, then this command assists you in determining your main branch and repository.
Generally, the term origin stands for the remote repository, and master is considered as the main branch. So, the entire statement "git push origin master" pushed the local content on the master branch of the remote location.
```
$ git push origin master  
```
