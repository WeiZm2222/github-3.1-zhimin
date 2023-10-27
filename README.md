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
- Uploads the local repository content to the main branch of your remote repository. This will transfer commits from the local repository to a remote repo.

## 7. git config
- Allows configuration of Git installation (or an individual repository) from the command line, includes user info, preferences, behavior of a repository etc
- git config --global user.email "you@example.com" : Define the author email to be used for all commits by the current user
- git config --global user.name "typeyourusername" : Define the author name to be used for all commits by the current user.

## 8. git branch
- List all of the branches in your repository
- git branch <nameofnewbranch> : Creates a new branch, but does not checkout into the branch
- git branch -d <nameofbranchtodelete> : Deletes the specified branch
- git branch -m <renamebranch> : Renames the current branch to the specified name

## 9. git diff 
- Shows all the local changes since last commit
- Git diff <filename> shows all the changes made to the specified file

## 10. git merge
- Takes the independent lines of development created by git branch and integrates/merges them into a single branch.

## 11. git rebase
- Combines a sequence of commits into a new base commit.
- git rebase --interactive <base> : Begins an interactive session which allows you to alter individual commits. Squash command is included here 

## 12. git reset
- Undo your last add to a staging area
- git reset --soft HEAD~1  : undo your last commit to a local repo. The soft command makes sure that the changes in undone revisions are preserved (i.e uncommitted local modifications in your working copy.)
- git reset --hard HEAD~1 : undo your last commit to local repo, but the hard command will delete everything (gone even from working directory)

## 13. git checkout＜branchname＞
- Allows you to navigate from current branch to <branchname>
- git checkout -b ＜new-branch＞ : Creates and checks out in to the new branch. The -b command tells git to perform git branch. 

## 14. git clean
- Deletes untracked files in a repo's working directory. Untracked files are files that have been created within your repo's working directory but have not yet been added to staging area. 

## 15: git log 
- Shows all commits in the current branch
- git log --oneline : Shows commits as a single line/summary

## 16: git status
- Displays the state of the working directory and the staging area. It lets you see which changes have been staged, which haven’t, and which files aren’t being tracked by Git.
