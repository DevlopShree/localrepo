# git bash!

Auther Shree Kant

0. pwd - to check your working directory 
0. git --version - to check git version

# Configuring Git
git config --global user.name "My Name"
git config --global user.email "someone@email.com"
git config --list
1. cd- To enter the inner folder of the folder cd means change directory (cd file_name)
        [(cd ..) to exit the the folder you are in]
2. ls - To list file the folder and to list all files includeing hidden file (ls -a)
3. git status - To check status of the folder
4. mkdir - to create a new file by git command (mkdir file_name)

# Work Flow of local Git (GitHub to LocalDisk)
github repo -> clone -> changes -> add -> commit -> push ->end
1. git clone - to clone a repo in pc first select the folder and then write
        (git clone repo_link)
2. git add - To add new or changed files in your working directory to the staging area 
        (git add file_name)  ad=nd to add all files (git add .)
3. git commit - it is the record of change (git commit -m"some_message")
4. git push - uplode local repo content to remote repo (git push origin main)
        use (git push -u origin main) to set the branch to push  the use  only (git push)

# Repo from local to git
1. git init - to add new repo from local to git (git init file_name) but first we need to make it git repo
2. git remote - to add new remote(repo) befor push (git remote add origin repo_link)
3. git remote -v - to verify remote
4. git branch - to check branch 
5. git branch -M - to rename the branch (git branch -M main)
6. git push - to push the file in the git
6. git log - to check all commits

for terminal error!!!
(Another git process seems to be running in this repository, problem) use int your terminal [rm .git/index.lock]

Git Branchs!

O------1------5------6 (main)---------
       |                             |-----7 (merge point)
       2------3------4 (feature1)------

# Branch Commands
1. git branch - to check which branch you are in.
2. git branch -m main - to change the name of the branch
3. git branch -d branch_name - to delete branch
4. git checkout - to to change brsnch or to navigate
5. git checkout -b new_branch_name - to create new branch

# Merging Code
way 1
1. git diff branch_name - to compare commits, branchs, files & more
2. git marge other_branch_name - to magre other branch to your branch

way 2 
1. create a PR(Pull request)
it lets you tell others about changes you pushed to a branch in a reposetory on GitHub.

# to add changes from repo to local
1. git pull oringin main - pull command

# undo changes
Case:
1. Stage changes (undo add)
        1. git reset file_name.
        2. fir reset (for all files)

2. Commit changes (for undo one commit)
        1. git HEAD~1
3. Commit changes (for many commits)
        1. Git reset commit_hash (hash is the commit id [use 'git log' to get])
        2. Git reset --hard commit_hash (to undo commit in your code editer)

# Frok
A fork is a ner repository that share s codes and visibility setting with the original "upstream" repository.
(fork is a rough copy of actual repository in your GitHub account) 