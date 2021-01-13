# GitHints
Hints for daily faced challenges in git.

# day 1 
push changes to remote repository

check the changes
git status

add files to index in order to make commit
git add .   - will add all changed files to index
git add [path to file]     - will add exactly file to index
git reset [path to file]   - will remove exactly file from index

make sure that all necessary files are added
git status

make loacal commit with message
git commit -m "[commit message]"       - will make commit with given message

push commit to the remote repository
git push origin HEAD

# day 2
chage message of last pushed commit 

git commit --amend -m "[New commit message.]"
git push --force origin HEAD

# day 3
remove some files from last pushed commit 

move back HEAD to previous commit
git reset --soft HEAD~1

check the changes
git status

remove useless files from this commit
git reset [path to file]

git push --force origin HEAD
