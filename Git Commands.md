# Git Commands

### Login to Github from terminal
1. 

### Create a new Respository on Github using terminal

1. `git init` : Transform the current directory into a Git repository.
2. `git init <directory>` : Transform a directory in the current path into a Git repository (e.g. Projects\*\Git-Terminal-Test is the current path and at this path, we have created a directory named 'Git-Repo'. git init Git-Repo will initialize Git-Repo as a repository and create a .git folder inside Git-Repo).
3. `git add .` : Make a readme file for the first commit and stage it using this command.
4. `git commit -m "First commit"` : Commit this file to make a first commit.
5. `git remote add origin <Repository_URL>` : Login to github and now you will see an empty repository. Copy the SSH or HTTPS URL and paste it in this command to add the origin to the local repository.
6. `git push -u origin master` : Use this command to push the changes to the remote repository. The -u sets the branch as upstream. Setting a branch as upstream makes the local branch to track the branch on the remote when multiple branches exists on the remote. In this command, we have made the master branch in the origin as the current upstream branch.
7. `git push <remote_name> <branch_name>` : The original syntax of the above command.

### Create a Repository on Github out of existing local repository

1. `git-init` : Inside the local repository, use this commmand to initialize a Git repository.
2. `git-init <directory>` : Transform a directory in the current path into a Git repository (e.g. Projects\*\Git-Terminal-Test is the current path and at this path, we have created a directory named 'Git-Repo'. git init Git-Repo will initialize Git-Repo as a repository and create a .git folder inside Git-Repo).
3. `git add .` : This command will stage the existing files in the local repository.
4. `git commit -m "First commit"` : Commit this file to make a first commit.
5. `git remote add origin <Repository_URL>` : Login to github and create a repository in the github. Copy the SSH or HTTPS URL and paste it in this command to add the origin to the remote repository.
6. `git push -u origin master` : Use this command to push the changes to the remote repository. The -u sets the branch as upstream. Setting a branch as upstream makes the local branch to track the branch (tracking branch) on the remote when multiple branches exists on the remote. In this command, we have made the master branch in the origin as the current upstream branch.
7. `git push <remote_name> <branch_name>` : The original syntax of the above command.

### Cloning a Git Repository

1. Go to the particular directory or folder where you want to clone a remote repository.
2. `git clone <Remote_Repository_URL>` : Now, add the URL of the Remote Repository you want to clone into this command and execute.

### Creating a new branch

1. `git checkout -b "<Branch_Name>"` : Insert the branch name that you want to use and execute this command to create a new branch.
2. Remember, the branch name must not exist alreaady on the remote otherwise it will simple just switch to that branch instead of creating a new branch. The -b flag simply tells git to run `git branch` before running this command.
3. `git fetch --all` : This commands fetches all the registered remotes and their branches.
4. `git branch` : Shows all the branches that exist on the remote.
5. `git checkout -b <branch_name> <existing_branch>` : By default, new branches are created from the current checked out branch (Head). Passing the extra parameter which is the existing branch name will enable git to create a new branch out of the head of that branch instead of the current checked out branch's head.

### Uninitializing the Git repository

1. `rm -rf .git` : Inside the repository that has been initialized earlier as a git repository, type this commmand to remove the .git directory and hence, uninitialize this repository as a git repository. Use git status to confirm that git is no longer tracking the repository. This command will work only in git bash.

### Git Commits

1. `git add .` : Stages all changed files to be committed.
2. `git restore --staged <file_name>` : Unstages all staged files preserving the changes back to local.
3. `git restore <file_name>` : Discards uncommitted local changes in the file and cannot be undone once executed.
4. `git reset` : Unstages all the staged files preserving the changes back to local.
5. `git reset -- <file_name>` : Unstages the staged file preserving the changes back to local.
6. `git reset --soft` : Just like above.
7. `git reset --hard` : Unstages all the staged file and removes the changes in the local.
8. `git reset <commit> -- <path>` :  Default commit value is HEAD. If specified, it will reset the index entries to the state at the specified commit hash.
9. `git status` : To check all the files which have been changed or are staged for commit.
10. `git commit -m "<message_body>"` : Commits the staged file with message body.
11. `git push -u origin <Branch_name>` : Pushes the commit to the specified branch in the remote. Using the -u flags sets the specified branch as the upstream branch and will be tracked by the local repository.

### Git updates

1. `git fetch` : This command will download all the content from the remote but will not update the local repository.
2. `git pull` : This command will download all the content from the remote and will also update the local repository.
3. `git fetch <remote_name>` : This command will download all the branches from the remote.
4. `git fetch <remote_name> <branch_name>` : This command will download all the content from the specified branch.
5. `git fetch -all` : This command will fetch all registered remotes and their branches.