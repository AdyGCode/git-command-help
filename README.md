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



