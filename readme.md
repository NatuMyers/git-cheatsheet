# Git Cheatsheet

## Delete branch both locally and remotely

```
git branch -D branch-name
git push origin --delete branch-name
```

## Merge branch without merge commit

```
git checkout master
git checkout -b feature/foo

# make some commits

git rebase master
git checkout master
git merge --ff-only feature/foo
```

[Source](http://stackoverflow.com/a/16358699/5147646)

## List remote branches

```
git branch -r 
```
