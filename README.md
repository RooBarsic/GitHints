# GitHints
Hints for daily faced challenges in git.

# day 0: Clone branch from remote repository

will clone only master branche
```git
git  clone  https://github.com/RooBarsic/GitHints.git
```

will clone branch with name "branch_name"
```git
git  clone  --branch  branch_name  https://github.com/RooBarsic/GitHints.git        -  
```

# day 1: Create new branch
* check branches that you already have
```git
git  branch
```
* Move to the base branch from which you want to create new branch ( usually it's master branch )
```git
git  checkout  BranchName
```
* create new branch
```git
git  branch  NewBranchName
```
* Move to the created branch
```git
git  checkout  NewBranchName
```

# day 2: Make commit and push changes to remote repository

* check the changes
```git
git  status
```

* add files to index in order to make commit
```git
git  add  .               - will add all changed files to index
git  add  PathToFile      - will add exactly file to index
git  reset  PathToFile    - will remove exactly file from index
```

* make sure that all necessary files are added
```git
git  status
```

* make loacal commit with message
```git
git  commit  -m  "commit_message"       - will make commit with given message
```

* push commit to the remote repository
```git
git  push  origin  HEAD
```


# day 3: Chage message of last pushed commit 

```git
git  commit  --amend  -m  "NewCommitMessage"
git  push  --force  origin  HEAD
```


# day 4: Remove some files from last pushed commit 

* move back HEAD to previous commit
```git
git  reset  --soft  HEAD~1
```
* check the changes
```git
git  status
```
* remove useless files from this commit
```git
git  reset  PathToFile
```
* push changes to remote repository
```git
git  push  --force  origin  HEAD
```

