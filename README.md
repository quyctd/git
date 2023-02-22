# GIT
A collection of Git commands that I hardly remember, and tired of searching over the internet anytime I need it.

### Get most recent (latest) active branches

```
git branch --sort=-committerdate
```

### Change commit time

```
GIT_COMMITTER_DATE="Wed Feb 16 14:00 2011 +0100" git commit --amend --no-edit
```

### Undo most recent commit
```
git commit -m "Something terribly misguided" # (0: Your Accident)
git reset HEAD~                              # (1)
# [ edit files as necessary ]                    # (2)
git add .                                    # (3)
git commit -c ORIG_HEAD                      # (4)
```

### Delete a branch
```
git push -d <remote_name> <branchname>
git branch -d <branchname>
```

### Revert code to specific commit, and create a new commit append to history

```
git checkout c8defdb .
git commit -m "NO-ISSUE Revert back to c8defdb"
git push
```
