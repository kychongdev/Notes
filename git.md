# Git command that might be useful one day

## Pull request on specific commit 
```
git fetch --all                                             # Get latest code
git checkout -b your-single-change-branch upstream/master   # Create new branch based on upstream/master
git cherry-pick yourcommitSHA                               # Cherry pick the commit you want
git push -u origin my-single-change-branch                  # Push your changes to the remote branch
```
Then create PR from that branch
<br>[Source](http://stackoverflow.com/questions/34027850/how-to-pull-request-a-specific-commit)

## Make small change after commit 
```
git add .                       # or add individual files
git commit --amend --no-edit
```
## Change commit message only
```
git commit --amend                      # Will open editor for commit message
git commit --amend -m "your message"    # this work too but harder to enter multi line
```
### DO NOT MESS WITH PUBLIC COMMIT WITH THESE
[Source](https://ohshitgit.com/#change-last-commit)
