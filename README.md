# My Git Command

> My Git Command in One File



```shell
  git init
  git config --local user.name "Sunel Tr"
  git config --local user.name "sunelbe@gmail.com"
  git config --local color.ui auto
  
```

```shell
  git config --local rerere.enabled true
  
```

if you have a branch that should always defer to upstream changes

```shell
  git config --local branch.master.rebase true
  
```

```shell
  git status -s

```

```shell
  git add -p

```

```shell
  
  git diff 
  
  git diff --stage
  
  git diff HEAD
  
```

```shell
  git reset --hard
  
```

```shell
  git log --oneline --decorate --all --graph 

```

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


```shell
  git reset --hard [commit id]
  
```

### Fast Forward Commit

```shell

  git checkout [branch]
  
  git rebase [master|develop]
  
  git checkout [master|develop]
  
  git merge [branch]
  
  #OR stop fast forward
  
  git merge [branch]  --no -ff

```
### To Rewrite History

```shell
  git rebase -i HEAD~[number of commit]

```
```shell
  git bisect start
  
  git bisect good [number]
  
  git bisect bad
  
  git bisect run [script to run with yes or no]
  
  git bisect reset
  
```
###Git Pull Causes a Merge

```shell
  git pull --rebase
  
```

```shell

```
```shell

```
```shell

```
