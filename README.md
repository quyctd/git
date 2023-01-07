# GIT
A collection of Git commands that I hardly remember, also tired of searching over the internet anytime I need it.

### Get most recent (latest) active branches

```
git branch --sort=-committerdate
```

### Change commit time

```
git commit --amend
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
