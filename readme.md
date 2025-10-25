## Learning Github

1. First of all you need to install Git in your system. You can download it from [here](https://git-scm.com/downloads)
2. Open Terminal
3. go inside your project folder using `cd <folder_path>`
    Follow the below steps to use Git commands for the first time


### 1. Add email firstly in terminal using 
`git config --global user.email "<your_email@example.com>"`

### 2. Add username using
`git config --global user.name "<your_username>"`

### 3. Initialize git repository using
`git init`

### 4. Check status using
`git status`

### 5. Add files to staging area using
`git add <file_name>` or `git add .` to add all files

### 6. Commit changes using
`git commit -m "your commit message"`

### 7. Link local repository to remote repository using
`git remote add origin <remote_repository_URL>` 
- Replace `<remote_repository_URL>` with your actual remote repository URL which you can find on your GitHub repository page in "Code" button.

### 8. Push changes to remote repository using
`git push -u origin master`
- You might be prompted to enter your GitHub username and password or a personal access token for authentication.
- After the first push, you can simply use `git push` for subsequent pushes.
- Make sure to replace `master` with `main` if your default branch is named `main`.
- That's it! You have successfully pushed your local changes to the remote GitHub repository.

## Additional Git Commands
- To pull changes from remote repository: `git pull origin master` (or `main`)
- To view commit history: `git log`
- To create a new branch: `git branch <branch_name>`
- To switch to a branch: `git checkout <branch_name>`
- To merge a branch into the current branch: `git merge <branch_name>`
- To clone a repository: `git clone <repository_URL>`
- To delete a branch: `git branch -d <branch_name>`
- To view the current branch: `git branch --show-current`
- To view remote repositories: `git remote -v`
- To remove a file from staging area: `git reset <file_name>`
- To discard changes in a file: `git checkout -- <file_name>`
- To view differences between working directory and staging area: `git diff`
- To view differences between staging area and last commit: `git diff --staged`
- To stash changes: `git stash` (This command saves your local modifications away and reverts the working directory to match the HEAD commit.)
- To apply stashed changes: `git stash apply` (This command reapplies the changes saved in the stash to your working directory.)
- To drop the most recent stash: `git stash drop` (This command removes the most recent stash entry.)
- To view all stashed changes: `git stash list` (This command lists all stashed changes.)
- To clear all stashed changes: `git stash clear` (This command removes all stash entries.)
- To rename the current branch: `git branch -m <new_branch_name>`
- To view the status of your repository including staged, unstaged, and untracked files: `git status`
- To view a summary of changes in a more concise format: `git status -s`
- To view a graphical representation of the commit history: `git log --graph --oneline --all`
- To amend the most recent commit (useful for fixing commit messages or adding forgotten changes): `git commit --amend`
- To delete a remote branch: `git push origin --delete <branch_name>`
- To fetch changes from the remote repository without merging: `git fetch origin`
- To reset the current branch to a specific commit: `git reset --hard <commit_hash>`
- To view the configuration settings: `git config --list`
- To set up a global .gitignore file: `git config --global core.excludesfile ~/.gitignore_global`   
- To view the differences between two branches: `git diff <branch1>..<branch2>`
- To tag a specific commit: `git tag <tag_name> <commit_hash>`
- To push tags to the remote repository: `git push origin --tags`
- To view all tags in the repository: `git tag`
- To remove a tag: `git tag -d <tag_name>` (for local) and `git push origin :refs/tags/<tag_name>` (for remote)
- To squash multiple commits into one: `git rebase -i HEAD~<number_of_commits>`
- To view the current stash contents without applying them: `git stash show -p`
- To configure Git to use a specific text editor for commit messages: `git config --global core.editor "<editor_command>"` (e.g., `code --wait` for VSCode) 
- To view the size of the repository and its objects: `git count-objects -vH`
- To clean untracked files from the working directory: `git clean -f` (use `-n` for a dry run to see what would be deleted)
- To view the blame information for a file (shows who made changes to each line): `git blame <file_name>`
- To configure Git to cache your credentials for a certain period: `git config --global credential.helper 'cache --timeout=<seconds>'` (e.g., `3600` for one hour)
- To view the differences between two commits: `git diff <commit_hash1> <commit_hash2>`
- To create and switch to a new branch in one command: `git checkout -b <new_branch_name>`
- and many more...
- There are total of over 200 git commands available. You can explore them in the [official Git documentation](https://git-scm.com/doc).

