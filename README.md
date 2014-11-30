# GDI upcoming events
#### Intermediate HTML and CSS / Intro to Responsive
December 6th 1pm - December 7th 5pm
Sendgrid - Boulder

#### Introduction to Distributed Systems
December 9th. 5:30-7:30pm
Dojo 4 - Boulder

---

# About your Instructors
Miles
* Senior developer at dojo4.com - 17th & pearl st behind Ted's. Stop by anytime!
* miles.matthias@gmail.com

Evan
* Full-stack dev in training at gSchool
* etmoore@gmail.com

---

# Initializing a Git Repository
1. Make a directory `$ mkdir <dir name>`
2. Move into the repository `$ cd <dir name>`
3. Initalize a git repository `$ git init`

---

# Essential Git Commands
### Create a new git repository
`$ git init` - Create a new, local repository

### Repo Status
`$ git status` - Check the status of your current repository and see which files have changed.

`$ git diff` - See the differences between your working tree and the latest commit.

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

---

# Basic Git Workflow
1. Do some work
2. `$ git status` to review your changes.
3. `$ git add <filename>` to add files to the staging area. (Use `$ git add -A` to add all files and changes.)
4. `$ git status` to see what you're about to commit
5. `$ git commit -m "<message>"` to commit the changes in the staging area with a message.

---

# Exercise 1 - Create and manage a local repo
1. Create a new directory 'song-lyrics'. `cd` into that directory.  
2. Initialize a git repository.
3. Create a new text file with the name of your favorite song. Example: `touch blank-space.txt`
4. Check the status of your repo to confirm that your new file exists and has not yet been added to your repo.
5. Add the new file to your staging area.
6. Commit the new file to you repo with the message "added \[filename\].txt to the repo"
7. Open the file in your text editor and write two lines of the song lyrics.
8. Check the status of your repo to see your changes.
9. Add your changes to the staging area.
10. Check the status to confirm that your changes have been added to the staging area.
11. Commit the changes to your repository with the message "first two lines"
12. Repeat steps 7-10, adding the third and fourth line of the song to what you already have written. Commit these changes with the message "third and fourth lines".
13. Repeat steps 7-10 one more time, adding the fifth and sixth lines. Commit changes with the message "fifth and sixth lines".
14. Run the fancy git log command (`git log --oneline --graph --decorate --all`) to see your commit history. You should see 4 commits. Congrats! You've completed the first exercise.

---

# Commands for working with a remote repository (e.g. Github)

`$ git clone <repo path or URL>` - clone a repository into a new directory.

`$ git remote` - List all remotes for the current repo.

`$ git remote add <remote name> <remote path or URL>` - adds a remote to your repo.

`$ git pull <remote name> <branch name>` - Pull down changes from a remote and integrate them into your repo. Performs `git fetch` and then `git merge`.

`$ git push <remote name> <branch name>` - Send your changes to the remote to be merged.

---

# Exercise 2 - Create and Manage a Remote Repository!
1. Log into your GitHub account
2. Create a repository on GitHub called 'song-lyrics'. (Don't initialize a readme). Copy the repo URL to your clipboard.
3. On your command line: Add the github 'song-lyrics' repo as a remote for your local 'song-lyrics' repo. Give the github repo the name `origin`.
4. Push your local commits up to github.
5. Go back to the GitHub song-lyrics repo (in your browser) and confirm that your commits were pushed... Congrats! You've made your first push to GitHub! Now your code is visible to the world.
6. In your text editor, write the first two lines if your song's chorus.
7. Check your repo's status, add, then commit the changes with the message "first two lines of chorus".
8. Push your changes up to Github. Confirm that the latest commit is there by looking at the commit history on GitHub.
9. In your text editor, finish writing the chorus.
10. Check the status of your repo, add, then commit the changes locally.
11. Push the changes up to GitHub.

Finished early? ...

1. Create a new file in your song-lyrics directory with the title of your second favorite song.
2. Add the file to be tracked by git.
3. Open the file in your text editor and make some changes.
4. Add, then commit the changes with a message of your choice. At this point, the file exists locally but does not exist in your remote repository. Confirm this by looking at your GitHub song-lyrics repo page.
5. Push your commits up to GitHub. You should now see the new file in your remote repo. Cool, eh?

---

# Exercise 3 - Collaborating with Github!
### Setup
1. Partner with 2 of your classmates to make a team of 3.
2. Decide who will be partner #1, #2, and #3.

### Part 1
Everyone:
1. Move out of your song-lyrics directory and create a new directory called 'gdi-haiku'.
2. `cd` into the 'gdi-haiku' directory and initialize a git repo.
3. Create a new file `<your first name>-haiku.txt`
4. Add the file to be tracked and commit with the message 'created haiku file'.
5. Open the .txt file in your text editor and write the _first_ line of the haiku. (Make it up! 5 syllables!)
6. Add, then commit your changes with the message "first line of haiku by [your first name]"
7. On GitHub, create a repo called 'gdi-haiku'.
8. Add the new GitHub repo as a remote called `origin`.
9. Push your local commits up to GitHub.
10. Confirm that your commits are now on GitHub.

STOP! Make sure your teammates have caught up before moving on to part 2.

### Part 2
1. Partner #1, go to partner #2's gdi-haiku GitHub repo and **fork** it. Partner #2, do this to partner #3. Partner #3, do it to Partner #1.
2. Clone the new forked repo (the url should have your username in it) to your computer.
3. Open your partner's haiku.txt file and write line 2 of the haiku. (Make it up! 7 syllables!)
4. Add, then commit the change to your local repo.
5. Push the change up to GitHub. Your change should now be reflected in your forked repo.
6. Click the green pull-request button. Review the changes. Click "Create Pull Request".
7. Give your pull request a title and (optional) comment. Click "Create Pull Request" to submit a pull-request to you partner.

Congrats! You've submitted your first pull-request!

STOP! Make sure your teammates have caught up before moving on to part 3.

### Part 3
1. Go to your gdi-haiku GitHub repo. You should see a pending pull-request from your partner. Review the pull-request and accept it if it looks good to you.

Congrats! You've accepted your first pull-request!

STOP! Make sure your teammates have caught up before moving on to part 4.

### Part 4
1. Repeat the steps in Part 2 and Part 3, but this time on your other partner's repo. Instead of writing the 2nd line of the haiku, you should be writing the 3rd and final line.
2. When finished, all three partners should a complete haiku, authored with two collaborators.

Nicely done!

---

# Advanced Git
**Aliases** - Make git commands easier and faster to type with command line shortcuts. For more: http://git-scm.com/book/en/v2/Git-Basics-Git-Aliases
**Rebasing** - Another way to merge that keeps your git history cleaner and more streamlined. For more: http://git-scm.com/book/en/v2/Git-Branching-Rebasing

---

# Additional Resources
Pro Git (free e-book) - http://git-scm.com/book  
Try git - https://try.github.io  
Github Training Videos - https://www.youtube.com/user/GitHubGuides  
Git for Ages 4 and Up (Video) - https://www.youtube.com/watch?v=1ffBJ4sVUb4  
A Practical Git Introduction - http://mrchlblng.me/2014/09/practical-git-introduction/  
Git Branching Game - http://pcottle.github.io/learnGitBranching/  
Github Guides - https://guides.github.com/
