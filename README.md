# GDI upcoming events

# About your Instructors
Miles  

Evan

# Initializing a Git Repository (Do this first!)
1. Make a directory `$ mkdir <dir name>`
2. Move into the repository `$ cd <dir name>`
3. Initalize a git repository `$ git init`

# Essential Git Commands
### Create a new git repository
`$ git init` - Create a new, local repository

### Repo Status
`$ git status` - Check the status of your current repository and see changes.

### Repo History
`$ git log` - Show all commits for the current branch, starting with the newest.

`$ git log --oneline --decorate --color --graph --all` - View the full tree history with an awesome commit graph, use  instead.

### Stage files to commit
`$ git add <filename>` - Add a file and its changes to the staging area.

`$ git add -A` - Add all files and changes to the staging area.

### Commit changes in staged files
`$ git commit -m "<commit message>"` - commit staged changes (the `-m` flag will let you add your commit message inline).

### Branching
`$ git branch <branch name>` - create a new branch

`$ git branch` - list all branches

`$ git checkout <branch name>` - switch to a different branch.

### Merging

`$ git merge <branch name>` - merge target branch into  current branch.

# Basic Git Workflow
1. Do some work
2. `$ git status` to review your changes.
3. `$ git add <filename>` to add files to the staging area. (Use `$ git add -A` to add all files and changes.)
4. `$ git status` to see what you're about to commit
5. `$ git commit -m "<message>"` to commit the changes in the staging area with a message.

# Commands for working with a remote repository (e.g. Github)

`$ git clone <repo path or URL>` - clone a repository into a new directory.


`$ git remote` - List all remotes for the current repo.

`$ git remote add <remote name> <remote path or URL>` - adds a remote to your repo.

`$ git pull <remote> <branch>` - Pull down changes from a remote and integrate them into your repo. Performs `git fetch` and then `git merge`.

`$ git push` - Send your changes to the remote to be merged.

# Advanced Git
Rebasing

Aliases
