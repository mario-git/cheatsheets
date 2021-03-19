Stage commands:

```
git add -f -- some-file-name.ext
git add -A	#stages All
git add .	#stages new and modified, without deleted
git add -u	#stages modified and deleted, without new
```

To remove an item from staging:

```
git reset -q -- some-file-name.ext
```

To show remote branches:

```
git branch -a
```

Global setup:

```
git config --global user.name "Name Surname"
git config --global user.email "name.surname@blah.world"
```

Set remote:

```
git remote add origin http://remoteurl.git
```

Change remote:

```
git remote set-url origin https://remoteurl.git
```

To remove local branches that aren't on remote:

```
git remote prune origin
```


Stash commands:
```
git stash save stashname
git stash pop --index 0
```

To delete a branch:

```
git branch -d local-branch-name
git push origin --delete remote-branch-name
```

To delete all branches exept main:

```
git branch | grep -v "main" | xargs git branch -D
```

To undo a commit:

```
git reset HEAD~
```

To show staged changes:
```
git diff --cached
```
