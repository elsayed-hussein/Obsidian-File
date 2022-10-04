## If git installed 
```bash
git --version
```

### Create empty git repository
```bash
git init
```

###  Check the status of git repo
```bash 
git status
```

### add files to the repo
```bash
git add <file/directory name 1> <file/directory name 2> < ... >
```
Or add all 
```bash
git add .
```

### Commit all the files that have been added along with message
```bash 
git commit -m "the message"
```

### add new remote 
```bash
git remote add origin https://<your-git-service-address>/owner/repository.git
```

### Clone repo
```bash
git clone https://github.com/username/projectname.git
```
or to Clone repo in folder 
```bash
git clone https://github.com/username/projectname.git MyFolder
```
or to clone repo in current directory
```bash
git clone https://github.com/username/projectname.git .
```