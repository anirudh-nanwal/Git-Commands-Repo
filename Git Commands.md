# Git Commands

### Login to Github from terminal
1. 

### Create a new Respository on Github using terminal

1. `git init` : Transform the current directory into a Git repository
2. `git init <directory>` : Transform a directory in the current path into a Git repository (e.g. Projects\*\Git-Terminal-Test is the current path and at this path, we have created a directory named 'Git-Repo'. git init Git-Repo will initialize Git-Repo as a repository and create a .git folder inside Git-Repo).

### Create a Repository on Github out of existing local repository

1. `git-init` : Inside the local repository, use this commmand to initialize a Git repository
2. `git-init <directory>` : Transform a directory in the current path into a Git repository (e.g. Projects\*\Git-Terminal-Test is the current path and at this path, we have created a directory named 'Git-Repo'. git init Git-Repo will initialize Git-Repo as a repository and create a .git folder inside Git-Repo)

### Uninitializing the Git repository

1. `rm -rf .git` : Inside the repository that has been initialized earlier as a git repository, type this commmand to remove the .git directory and hence, uninitialize this repository as a git repository. Use git status to confirm that git is no longer tracking the repository.

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
