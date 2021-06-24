# PR Process

## Confirm your git history is clean
  * `git fetch`
  * `git status`
### If you are *behind* then you need to catch up
  * `git pull`
### If you are *ahead* then you need to save your changes
  * `git stash push`
#### Then change to the branch you meant to be on
 * `git checkout feature/branch-name`
#### Load your saved changes
 * `git stash pop`
## Make a branch 
  * `git checkout -b feature/branch-name`
## Make whatever changes to the code you mean to make
## Confirm that the files you edited are changed, and that there aren't changes you don't expect
  * `git status`
## Maybe add untracked files to branch
 * `git add path/to/file.name` **or** `git add *`
## Commit changes
  * `git commit -a -m "commit message here"`
## Push changes to github
  * `git push --set-upstream origin feature/branch-name`
    * Don't worry if you forgot this command, if you `git push` git will give that exact same command to you to cut and paste
## Create a pull request to add changes to main branch
  * On webpage, click **Pull Requests**
  * There are two dropdowns, the left should be `main` the right should be changed to the branch you want to have merged in
  * Click **Create Pull Request**
## Add a description of what you did.  
### This should be thorough and readable by your teammates
### You should also include a way to confirm the changes are working as intended and not just silently doing something wrong or weird
  * Click **Create Pull Request**
## While you are on the website, approve any outstanding PRs from your teammates, after checking them out and thoroughly testing them of course (or at least reading the changes and making sure they make sense)
