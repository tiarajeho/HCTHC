

## Content

### What is the difference between push, pull, and fetch?

- `git fetch` - sends changes from a remote repository to your tracking branch
- `git pull` - sends changes from a remote branch to your tracking branch and merges them into a local branch
- `git push` - sends changes from your local branch to a remote repository

`git fetch` takes your current branch and checks for a tracking branch, then takes the changes from the remote branch and pulls them into your tracking branch. It does not change your local branch. To do that, you'll need to do a `git merge origin/master` (for the "master" branch) to merge those changes into your branch. `git pull` does a `git fetch` followed by a `git merge`. We recommend using this method if you want to see the changes made to your branch before they are merged. `git push` checks your current branch for a tracking branch connected to a remote repository, and pushes changes from your current branch to your remote branch. This is how code is shared with a remote repository to make your remote branch resemble your local one. Use `git pull`, `git fetch`, or `git merge` to sync your local branch with the remote branch to ensure a smooth process. 
