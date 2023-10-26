# github-3.1-zhimin
## Assignment 3.1 :Introduction to GIT I

 Github commands learnt and what they are used for: 
## 1. git init
 - One-time command you use during the initial setup of a new repo. 
 - Transforms the current directory into a Git repository. Creates a new .git subdirectory in the current working directory. Creates a new main branch and makes it possible to start recording revisions of the project.

## 2. git clone <ssh or https of remote repo>
 - Clones the repository specified into the local machine. Cloning automatically creates a remote connection called "origin" pointing back to the original repository.
 - Usually a 1 time operation

## 3. git pull
 - Fetches and downloads content from a remote repository and immediately updates the local repository to match that content
 - git pull command is actually a combination of "git fetch" and "git merge". The git fetch command copies changes into your local Git repo. The git pull command will ensure it is copied into your working directory as well. git pull will first execute a git fetch scoped to the local branch that HEAD is pointed at. Once the content is downloaded, git pull will enter a merge workflow. A new merge commit will be-created and HEAD updated to point at the new commit.

## 4. git add
- Adds a change in the working directory to the staging area

## 5. git commit -m "type-commit-msg-here"
 - Captures a snapshot of the project's currently staged changes, with -m allowing you to enter a commit message

## 6. git push origin main
- Uploads the local repository content to the main branch of your remote repository. This will transfer commits from the local repository to the remote repo.
