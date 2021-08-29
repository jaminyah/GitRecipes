# GitRecipes

```bash
1. Remote
1.1 Check the Upstream
1.2 Show the Remote
1.3 Change the Remote Origin

2. Manage Local Repositor
2.1 Delete Branch
2.2 Abort Merge
2.3 Stash Changes
2.4 Apply Stashed Changes
2.5 Git Unstage
2.6 Discard Working Directory Changes
2.7 Remove project from Git Directory
2.8 Remve DS_Store from cache
```

A collection of commands encountered when using Git.

1.1 Check the Upstream
```bash
git remote show origin
```

1.2 Show the Remote
```bash
git remote -v
```

1.3 Change the Remote Origin

1.3.1 Option - 1
Remote the local remote and add the new remote.
```bash
git remote -v                   # show remote
git remote remove origin
git remote -v
git remote add <url>            # GitHub - url: https://[token]@github.com/[username][repo]
git remote -v
```
1.3.2 Option - 2
Use set-url
```bash
# git remote set-url <name-of-the-remote> <url-address-of-remote>
git remote set-url origin https://[token]@github.com/<username>/<repo.git>
```


2. Manage Local Branch
2.1 Delete Branch
```bash
git branch -d <branch-name>
```

2.2 Abort Merge
```bash
git merge --abort
```

2.3 Stash Changes
```bash
git stash
```

2.4 Apply Stashed Changes

2.4.1 Apply without deleting stash
```bash
git stash apply
```

2.4.2 Apply and delete stash
```bash
git stash pop
```

2.5 Git Unstage
```bash
git rm --cached <filename>
```

2.6 Discard Working Directory Changes
```bash
git restore <filename>
```

2.7 Remove project from Git Directory
```bash
rm -rf .git
```

2.8 Remve DS_Store from cache
```bash
git rm --cached -f *.DS_Store
```