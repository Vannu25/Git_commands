# Git_commands

### Getting started - GIT STAGE
 - git init
 - git status - show modified files in the working directory, staged for your next commit
 - git add . (add all files to the staging area)
 - git reset FILE_NAME.extension  (Unstage file from staging area)
 - git commit -m “[descriptive message]"
 - git branch -M master  (Create master branch)
 - git push -u origin master  (push the newly created master branch to remote)
 - git pull (pull changes from remote to local)
 - git diff - diff of what is changed but not staged


 ### Show commit logs
  - git log --stat
  - git log --oneline --graph --decorate --all
  - git log
  - git show [SHA]
  
  
 ### Working with tag
  - git tag -a v0.1 -m "meaningful comment" COMMIT_ID  (creates tag locally)
  - git push --tags (push all created tags to remote)


### Git config and SETUP
 - git config --list  (view all config settings)
 - git config --global user.name “[firstname lastname]"
 - git config --global user.name “[firstname lastname]"
 - git init
 - git clone [url]
 
### Local and remote repp
 - git remote -v (list all linked remote repo)
 - git remote set-url origin repo-URL  (set new remote repo)
 - git remote add [alias] [url]
 - git push [alias] [branch]
 
### Branches
 - git branch - list your branches
 - git checkout branch-name
 - git branch --merged (check if any branch merged with current)
 - git checkout -b branch-name (create a new branch and switch to it)
 - git branch -d dev   (Delelet local branch)
 - git branch -D dev   (Delelet local branch forcefully)
 - git push --delete origin dev  (Delete remote branch)
 - git merge [branch]
 
### Revert commit
 - git revert commit_id

### Changes in file
- git diff  (difference in the file)

### Stash
- git stash
- git stash list
- git stash apply stash@{0}
- git stash pop entry index  (apply and delete)
- git stash apply entry index 
- git stash drop entry index  (delete)
- git stash clean

### Create alias
- git config --global alias.am "!git add -A && git commit -m"
- git am "new message"  (will do samething as above two command using am alias)
- git config --global --unset alias.am (unset alias created in config file)
