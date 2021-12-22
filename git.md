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