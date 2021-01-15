# GitHints
Hints for daily faced challenges in git.

# day 0: Clone some branch from remote repository

will clone only master branche
```git
git clone https://github.com/RooBarsic/GitHints.git
```

will clone branch with name "branch_name"
```git
git clone --branch branch_name https://github.com/RooBarsic/GitHints.git        -  
```

# day 1 
push changes to remote repository

* check the changes
```git
git status
```

* add files to index in order to make commit
```git
git add .   - will add all changed files to index
git add [path to file]     - will add exactly file to index
git reset [path to file]   - will remove exactly file from index
```

* make sure that all necessary files are added
```git
git status
```

* make loacal commit with message
```git
git commit -m "[commit message]"       - will make commit with given message
```

* push commit to the remote repository
```git
git push origin HEAD
```


# day 2
chage message of last pushed commit 

```git
git commit --amend -m "NewCommitMessage"
git push --force origin HEAD
```


# day 3
remove some files from last pushed commit 

* move back HEAD to previous commit
```git
git reset --soft HEAD~1
```
* check the changes
```git
git status
```
* remove useless files from this commit
```git
git reset [path to file]
```
* push changes to remote repository
```git
git push --force origin HEAD
```

