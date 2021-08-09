# Git Demo

This is a demo git repo with a list 
of commands as a cheat sheet.

## Creating a Local Repo

1) Change into the required folder:
   PC:
   ```bash
   cd %HOME%\Source\Repos
   ```
   MAC:
   ```bash
   cd ~/Source/Repos
   ```

2) Create New Folder
    ```bash
   mkdir Project-Name
   ```
3) Change into the new folder
   ```bash
   cd Project-Name
   ``` 
4) Initialise with Git
```bash
   git init
```
5) Change Master to Main (moves the branch to new name)
```bash
git branch -m master main
```
6) Check the status
```bash
   git status
```   
7) Create a `.gitignore`
MAC:
```bash
   touch .gitignore
```
PC:
```bash
   echo "" > .gitignore
```
8) Add required "ignores" to the `.gitignore` file. Recommend that you use a known .gitignore 
   or head to [http://gitignore.io](http://gitignore.io)
9) Check the status
```bash
   git status
``` 
10) Add and Commit the ignore file to version control
```bash
   git add .gitignore
   git commit -m "Original Commit"
```
11) Verify commit
```bash
   git status
``` 
Aside: we added a README.md (This file) at this point, and added it to Version Control.

### Adding files to Tracking
```bash
git add filename
git add foldername/*
git add -A
git add .
```

### Checking the Logs
```bash
   git log
```

### Create a Branch
```bash
   git branch Branch-Name
```

### Change Branches
```bash
   git checkout Branch-Name
```

### Merging changes from one branch into main
```bash
   git checkout main
   git status
   git merge Branch-Name-To-Bring-In
   git status
   git log
```

## Remote Repositories
Before you can use a remote repository (repo) you need to have created it on the remote system.

We will use GitHub for this purpose, other remote repositories that use Git are also valid.

## Create a Remote Repo
1) Head to https://github.com
2) If you do not have an account, create a github account
3) Create a new repo making sure that:
   - Do not add a README.md
   - Do not add a License
   - Do not add a .gitignore
   - In other words: Do not add anything to the **blank** repo.

### Connecting a Remote Repo
```bash
git remote add origin https://github.com/ACCOUNT_NAME/REPO_NAME.git
```
origin = alias for the remote

### Pushing commits to the remote
```bash
git push -u origin main
```





## Asides!

### Markdown Table

| Heading 1 | Heading 2 | Another Heading |
|---|---|---|
|Content for Cell| Another bit | Last bit |
|Another row... | | |
