# HappyGitScenario
A git scenario to start using git quickly.

### Why ?
It may be your first time using Git, and you don't have enough time to learn everything about it.

This scenario will likely get you running using git in safe and quick manner. But that's not intended to replace any learning ressources on the internet, it is just to get you starting happilly quickly!

### Scenareo
* Clone a repo
```
git clone https://github.com/elhoucine/HappyGitScenario.git
```

* Or create a git repo:
```
git init
```

* List all branches:
```
git branch
```

* Download or fetch a remote branch:
```
git fetch origin develop
git checkout develop
```

* Create a new local branch:
```
git branch new-Branch
```

* Checkout to a branch:
```
git checkout existing-Branch
```

* Create a new local branch and checkout to it:
```
git checkout -b another-New-Branch
```

* Update local branch with remote branch:
```
git pull origin develop
```

* Push a local branch to remote:
```
git push origin new-Branch-Name
```

* Merge a branch into another one:
```
git checkout branch-I-want-To-Merge-To
git merge branch-I-want-To-Merge
```

* Committing:
```
git status             # See what's going on.
git add fileName       # or (git add .) for all listed files.
git commit -m 'commit message'
```

* List all commits:
```
git log --oneline
```

* Revert to a previous commit:
```
git revert commit-Id
```

* Update the last commit message:
```
git commit --amend
```

* Rename a local branch:
```
git checkout branch-I-want-To-Rename
git branch -m newName
```

* Remove a local branch:
```
git branch -D branch-To-Remove
```

* Remove a remote branch:
```
git checkout origin :remote-Branch-To-Remove
```


### Happy Git ref:
- [ ] RELAXING git workflow.
- [ ] SSH.
