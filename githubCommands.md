# **GitHub**
**What is GIT**  
Version control system (VCS) for tracking changes in computer files  
- Distributed version control
- Coordinates work between multiple developers
- Who made what changes and when
- Revert back at any time
- Local & remote repos  

**Concept of GIT**
- Keeps track of code history
- Takes "snapshots" of your files
- You decide when to take a snapshot by making a 'commit'
- You can visit any snapshot at any time
- You can stage files before committing

### Basic Commands
```
    git init
    git add .
    git rm --cached filename.extension
    git status
    git commit -m 'Comment'

    git push
    git pull

    git clone

    git remote
    git push -u origin master
    git remote rm origin

    touch .gitignore

    git checkout -b <branch-name>

    merge branch
    first checkout to master
    git checkout master
    git merge desktop
    git merge container
    git push -u origin master
    
```

### **Details**
>Initialize local Git Repository. It will create a Git folder in the repository hidden by default

    `$ git init`

>### Add files to index

    `$ git add <file>`
    `$ git add *.extension` 
    `$ git add .` To add every thing
    When some modification is performed again use git add . to add the changes to staging area

>### Remove from staging area 

    `$ git rm --cached filename.extension`

>### Check status of working tree 

    `$ git status`

>### Commit changes in index

    `$ git commit` 
    `$ git commit -m 'Comment for your self'`
    `$ git commit -m 'Changes done in index file'`
    `$ git commit -m 'changed <filename.extension>'`

>### Push repository and pull repository 

    `$ git push` 
    `$ git pull` 
  

>### Ignore Files for commit

    `touch .gitignore`
    
    Create a file without name just an extension of gitignore
    Open the file .gitignore and just enter the complete filename that you want to ignore. 
    ---
    Multiple files can be added in the '.gitignore' file by simply putting a forward slash after the filenames.
    
    `.env/node_modules` 


>### Push to remote repository

    `$ git push`

>### Pull latest from remote repository 

    `$ git pull`

>### Clone repository into a new directory 

    `$ git clone`

>### Creating branches
``` github
git checkout -b <branch-name>
git branch <nameOfTheBranch>` Create a branch
git checkout <nameOfTheBranch>` Login to another branch
git merge <nameOfTheBranch>` Should be in master branch to perform
git branch -M master`
```

>### List remote repository 12

    `git remote` To list repositories
    `git remove rm <name of repository>`
    


>### Clone repository into a new directory 

    `$ git clone`

>### Git remote connection

    `$ git remote add origin https://`
    `$ git push -u origin master`
    `$ git remote rm origin` To remove repos


### **Installing Git**
>Windows 

    http://git-scm.com/download/win`
 
### Conflict with merge
```
https://www.youtube.com/watch?v=XX-Kct0PfFc
time 7:38
```

### Git reset command
```
git reset --soft HEAD^
```


### Remove single or multiple docker images
```docker
docker rmi <image-id>
docker rmi <image-id> <image-id> ...
``` 

### config 
```
git config -l
```

### Commands
```
1. change from master to other branch
2. git pull origin master
    IF Error 
    commit your changes or stash them before you merge
    git checkout HEAD fileName
```