# Git Milestones - Advanced

Below is a list of tasks if you want to deepen your understanding of Git.



## Git Fluency

The following are not required for DIG 245, but if you would like to improve your Git knowledge then carry forth!


### Top 20 Git Commands
You should be able to explain what each of these do:

*Starting up*
- [x] [`git config`](# "Set the author name and email to be used with your commits")
- [x] [`git init`](# "Create a new local repository")
- [x] [`git clone <url>`](# "Check out a repository")

*Workflow*
- [x] [`git status`](# "List the files you've changed and those you still need to add or commit")
- [x] [`git diff`](# "Preview changes, before merging")
- [x] [`git add <filenames>`](# "Add one or more files to staging")
- [x] [`git commit -m "message"`](# "Commit changes")

*Remote*
- [x] [`git push`](# "Send changes to the master branch of your remote repository")
- [x] [`git pull`](# "Fetch and merge changes on the remote server to your working directory")
- [x] [`git remote`](# "List all currently configured remote repositories")

*Branching*
- [x] [`git branch`](# "List all the branches in your repo, and also tell you what branch you're currently in")
- [x] [`git checkout -b <branchname>`](# "Create a new branch and switch to it")
- [x] [`git checkout <branchname>`](# "Switch from one branch to another")
- [x] [`git merge`](# "To merge a different branch into your active branch")

*Maintaining order*
- [x] [`git reset`](# "Unstages files, preserving the file contents")
- [x] [`git rm <filename>`](# "Delete the file from your working directory and stages the deletion")
- [x] [`git log`](# "List the version history for the current branch")
- [x] [`git show`](# "Show the metadata and content changes of the specified commit")
- [x] [`git tag`](# "You can use tagging to mark a significant changeset")
- [x] [`git stash`](# "Temporarily stores all the modified tracked files")





### Fetch from Upstream
You should be able to sync a fork of a repository to keep it up-to-date with the upstream repository.

- [ ] With Github Desktop...
  - [ ] While in the default branch (`master`) switch to the history tab
  - [ ] Select the branch called `upstream/master` and click "Merge into master"
- [ ] Or, on command line
  - [ ] Fetch project branches from the upstream repository to get all the commits:
  ```
  git fetch upstream
  ```
  - [ ] Check out the master branch from your local fork
  ```
  git checkout master
  ```
  - [ ] Merge the changes from `upstream/master` into your local `master` branch. Your fork’s master branch will be in sync with the upstream repository. You will not lose your local changes:
  ```
  git merge upstream/master
  ```
