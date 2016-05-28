# Git Cheatsheet



## Initial
Makes current directory a git repo (after you make a git repo on github.com first!)

```
git init 
git add .
git commit -m "init"
git remote add origin URLHERE
git push -u origin master
```


## Post Initial Push (same minus git init)

```

git add .; git commit -m "update"; git remote add origin URLHERE; git push -u origin master
```


## Make a branch

```

git checkout -b [name_of_your_new_branch]
git push origin [name_of_your_new_branch]
```


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
