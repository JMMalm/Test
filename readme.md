# Test
This is a test repo for practicing Git.

## Basics
1. Current status: `git status` or `git status -s` for the short version.
2. Add changes: `git add <filename>` or `git add .` to add all.
  * Remember that new modifications to staged file(s) must be re-added.
3. Commit changes locally: `git commit -m "Commit message."`
4. Push changes: `git push origin <branch>`

## Updating & Merging
* Get latest: `Git pull`
* Merge another branch into the active branch: `git merge <branch>`
* To preview merge changes: `git diff <sourceBranch> <targetBranch>`
* Replace local change(s): `git checkout -- <fileName>` (replaces with most recent content in HEAD)
* Replace ALL local changes (caution!):
  1. `git fetch origin`
  2. `git reset --hard origin/master`

## Branching
* View local branches: `git branch`
* Create and checkout new branch: `git checkout -b <branchName>`
* Switch to existing branch: `git checkout <branchName>`

### Stashing
* Save changes and revert to clean workspace: `git stash`
* List stashes: `git stash list`
  * These are specific to each branch.
* Show more stash detail: `git stash show`
* Apply stashed changes: `git stash pop`
  * Throws away the stash after successfully applying the changes.
  * Use `git stash apply` to apply stashed changes and *keep* the stash.

### Visualization
* View a graph of branches and commits: `git log --graph --decorate --oneline`

### Conflicts
1. Manually sort out the conflict changes.
2. Mark the changes as "merged" via: `git add <mergedFileName>`

## History
* All changes: `git log`
  * Press `q` to or `q + Enter` (Windows) to quit.
* Compressed history: `git log --pretty=oneline`