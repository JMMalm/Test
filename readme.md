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

### Conflicts
1. Manually sort out the conflict changes.
2. Mark the changes as "merged" via: `git add <mergedFileName>`

## History
* All changes: `git log`
  * Press `q` to or `q + Enter` (Windows) to quit.
* Compressed history: `git log --pretty=oneline`