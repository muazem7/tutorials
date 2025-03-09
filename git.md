# Git commands

## Configuration

Use the ssh-keygen command to create GitHub SSH key pairs:
```sh
cd ~/.ssh
ssh-keygen -o -t rsa -C "your.email@example.com"
```

Copy the contents of the id_rsa.pub file to your clipboard
```sh
cat ~/.ssh/id_rsa.pub | clip
```

Set user email for local directory, single project:
```sh
git config --local user.email "your.email@example.com"
```

Set user name:
```sh
git config --global user.name "Your Name"
```

Set user for all git projects:
```sh
git config --global user.email "your.email@example.com"
```

Check current configuration:
```sh
git config --list
```
Create an alias named gc for the “git commit” command
```sh
git config --global alias.gc commit
gc -m "new commit"
```

## Repository Initialization

Initialize a new Git repository:
```sh
git init
```

Create a Git-tracked repository inside a new directory
```sh
git init <dir_name>
```

Clone an existing repository:
```sh
git clone <repo_url>
```

Clone only a specific branch:
```sh
git clone --branch <branch_name> <repo_url>
```

Clone into a specified directory:
```sh
git clone <repo_url> <dir_name>
```

## Staging and Committing

Check repository status:
```sh
git status
```

Add files to staging area:
```sh
git add <file>
```

Add all changes to staging:
```sh
git add .
```

Commit staged changes:
```sh
git commit -m "Commit message"
```

Remove file from working directory and staging area:
```sh
git rm <file>
```

To remove a directory (and all its contents):
```sh
git rm -r mydirectory/
```

Unstage and remove paths only from the index (stop tracking the file):
```sh
git rm --cached <filename_or_dir>
```

## Branching and Merging

List all branches:
```sh
git branch
```

Create a new branch:
```sh
git branch <branch-name>
```

Switch to a branch:
```sh
git checkout <branch-name>
```

Create and switch to a new branch:
```sh
git checkout -b <branch-name>
```

Merge a branch into the current branch:
```sh
git merge <branch-name>
```

Delete a branch:
```sh
git branch -d <branch-name>
```
 
Delete a remote branch:
```sh
git push <remote_repo> --delete branch
```

## Remote Repositories

Add a remote repository:
```sh
git remote add origin <repo_url>
```

Remove a connection to a remote repo called <remote_repo>:
```sh
git remote rm <remote_repo>
```

Rename a remote connection:
```sh
git remote rename <old_name> <new_name>
```

Check remote repositories:
```sh
git remote -v
```

Fetch changes from a remote repository:
```sh
git fetch
```

Push changes to a remote repository:
```sh
git push origin <branch-name>
```

Pull latest changes from a remote repository:
```sh
git pull
```

## Undoing Changes

Unstage a file:
```sh
git reset <file>
```

Undo last commit but keep changes:
```sh
git reset --soft HEAD~1
```

Undo last commit and remove changes:
```sh
git reset --hard HEAD~1
```

Revert a commit:
```sh
git revert <commit-hash>
```

## Logs and History

View commit history:
```sh
git log
```

show the commits on branchA that are not on branchB:
```sh
git log branchB..branchA
```

View commit history in one line:
```sh
git log --oneline
```

Check who changed what in a file:
```sh
git blame <file>
```

Show differences between commits/files:
```sh
git diff branchB...branchA
```

Show last commit changes:
```sh
git show <commit_SHA>
```

## Stashing

Save changes without committing:
```sh
git stash
```

List all stashes:
```sh
git stash list
```

Apply latest stash:
```sh
git stash pop
```

Discard the changes from top of stash stack:
```sh
git stash drop
```

Apply specific stash:
```sh
git stash apply stash@{n}
```

## Tags

Create a new tag:
```sh
git tag <tag-name>
```

List all tags:
```sh
git tag
```

Push tags to remote repository:
```sh
git push --tags
```