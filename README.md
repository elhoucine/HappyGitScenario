# HappyGitScenario
A git scenario to start using git quickly.

[Read it on Meduim.](https://medium.com/@byjmlays/a-git-short-movie-e4931af229e3#.avlmlstmh)

## Why ?
It may be your first time using Git, and you don't have enough time to learn everything about it.

This scenario will likely get you running using git in safe and quick manner. But that's not intended to replace any learning ressources on the internet, it is just to get you starting happilly quickly!

Note: `git help #Anything after # is just a comment and it's ignored by git`.

## Scenario
## Repos

#### Clone a repo
```
git clone https://github.com/elhoucine/HappyGitScenario.git
```

#### Or create a git repo:
```
git init
```

## Branches

#### List all branches:
```
git branch
```

#### Download or fetch a remote branch:
```
git fetch origin develop               #fetch from server
git switch develop                     #link with a local branch
```

#### Create a new local branch:
```
git branch newBranch                   #new branch only on my machine
```

#### Move to another branch:
```
git switch existingBranch
```

#### Create a new local branch and checkout to it:
```
git switch -c newBranch                 #now I am in newBranch
```

#### Get updates from the server:
```
git pull origin develop                 #will download the latest changes from the server into develop
```

#### Push my local branch to the server:
```
git push origin newBranch
```

#### Merge a branch2 into branch1:
```
git switch branch1
git merge branch2
```

## Commits:

#### Committing:
```
git status                             # See what's going on.
```

The above will print you files in red and-or green, green are ready to be commited, red should be added first, see below.

```
git add file1 file2                    # To add only specific files
```
OR
```
git add .                              # Add all changed files
```

You may want to use `git status` again to make sure what files are stagged for commit, then:

```
git commit -m 'commit message'         # memorise my changes.
```

This is the short commit form, you can use `git commit` only for advanced message.


#### List all commits:
```
git log --oneline                       #remove --online to see full commit details.
```

#### Revert to a previous commit:
```
git revert commitId 
```

> revert does not reset previous changes, it undo them in a new commit instead, it's less dangerous than `reset`.

#### Update the last commit message:
```
git commit --amend
```

> This will let you update the content of the last commit and may result in converging with remote branch, only use when your last commit is not pushed.  

## Utilities:

#### Rename a local branch:
```
git switch branhc2
git branch -m branch2
```

> You should be pointing at the branch you want to rename.

#### Remove a local branch:
```
git branch -d testBranch                     #It will only work if testBranch was pushed and merged so it's safer to use.
```

> The param -d is case sensitive, the lowercase -d option is a safe delete and will give you useful warnings.
> Don't use the capital option -D because it's a force delete and can delete your hard work accidentally.

#### Remove a remote branch:
```
git checkout origin :remoteBranch            #Dangerous, never do this.
```

> Never try to remove a remote branch from your local machine, you may accidentaly remove someone else's or an important (non protected) branch.
> An alternative is to remove remote branches from the git platform carefully.


### Happy Git ref:
- [ ] RELAXING git workflow.
- [ ] SSH.
