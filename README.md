# My Git Command

> My Git Command in One File



```shell
  git init
  git config --local user.name "Sunel Tr"
  git config --local user.email "sunelbe@gmail.com"
  git config --local color.ui auto
  
```

#### Same merge conflict every time

```shell
  git config --local rerere.enabled true
  
```

##### If you have a branch that should always defer to upstream changes

```shell
  git config --local branch.master.rebase true
  
```

#### To check status in short
```shell
  git status -s

```

#### Only stage commits that you need interactively 
```shell
  git add -p

```

#### Ignore watching/tracking a particular dir/file
```shell
  git update-index --assume-unchanged <file>

```


#### Edit an incorrect commit message
```shell
git commit --amend -m "New commit message"

````

#### Unstage your files 
```shell
  git reset --hard
  
```

#### Unstage your files interactively
```shell
  git reset  -p
  
```

#### Diff your commits
```shell
  
  git diff #diff unstaged files
  
  git diff --stage #diff staged files
  
  git diff HEAD #diff both files
  
```

#### View git log
```shell
  git log --oneline --all --decorate --graph --pretty=format:"%h - %an [%ar] : %s"

```
#### Steps to merge 
```shell
  git merge [branch]
  #if conflict then
  
    git merge --abort
  
    #OR
  
    git status 
  
    vi [file]
      #search for the =====
      /====
  
      #resolve the conflict
      #press "n" to find the next one 
      #repeat unitl all are resloved
  
      n
  
      #save the file 
      :wq
  
    git add 
    git commit
  
  #else
  #Bro Fist

```

#### Reset the merged commits
```shell
  git reset --hard [commit id]
  
```

#### To get all deleted file list 

```shell
  git log --diff-filter=D --summary | grep delete
  
  git log --all -- <path-to-file>
  
  git show <SHA> -- <path-to-file>
  
```

#### Fast Forward Commit

```shell

  git checkout [branch]
  
  git rebase [master|develop]
  
  git checkout [master|develop]
  
  git merge [branch]
  
  #OR stop fast forward
  
  git merge [branch]  --no -ff

```
#### To Rewrite History

```shell
  git rebase -i HEAD~[number of commit]

```

#### To search in old commits 

```shell
  git bisect start
  
  git bisect good [number]
  
  git bisect bad
  
  git bisect run [script to run with yes or no]
  
  git bisect reset
  
```
### Git Pull Causes a Merge

```shell
  git pull --rebase
  
```
#### To view all commites for a file 

```shell
  git log --follow filename
  
```
