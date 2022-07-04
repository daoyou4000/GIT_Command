# GIT_Command
  Put a few popular git command here. 
- git log
  
  shows the commit trace log in the repository. 
- git status
  
  compare your local copy with remote repository. it shows which file is modified.
- git add .
   
  add the file you hope to upload, 
- git commit -m "comment you prefer to show the readers"
- git push
  
  push your commit to the remote repository and the whole modification process is done here.
- touch .gitigore


  build the one script for git that runs for git, it will igore the file that does need to be committed.
  
  e.g., it will ignore the files with postfix .lst and .s in  
    
    Debug/Obj/
   
    **/*.lst
    **/*.s

- git commit --amend 

  it is used to modify the commit messages. 

- git reset HEAD

  reset the pointer to the HEAD.

-  git rev-parse --short HEAD

  this the command that to get the short hash.

- git checkout Branch_Bootloader_And_Fwupdate

  The **git checkout** is used switch in between different branchs. 

### multiple branches in the GIT

- first **git clone** the master branch then **git checkout BRANCHNAME**

- Then do some other operations.

- **alias** 用法， 使用简短指令 
    
    e.g., alias gitlog = 'git log --pretty=format:"%h%x09%an%x09%ad%x09%s"'
    当使用 **gitlog** 指令时会运行后面的一堆指令。
    
### Git cover the code in local copy 覆盖当前本地文件    
- ````git fetch --all````
- ````git reset --hard origin/master```` 覆盖master分支
- ````git reset --hard origin/<branch_name>```` 覆盖branch分支

### Use the Git to merge the two branches. 

Use GIT to merge multiple branches might be the best way. [Link](https://www.varonis.com/blog/git-branching#:~:text=To%20merge%20branches%20locally%2C%20use,branch%20into%20the%20main%20branch.)
- Step 1, Build one new repository and **git clone xxxxx**
- Step 2, **git checkout** both branches 
- Step 3, enter the master branch 
- Step 4, **git merge** the other branch 
- Step 5, There would be some conflicts, use the IDE to compile the result and resolve the conflicts.

### git pull -r
when you start using your local workspace then commit and see the diverge the problem.
This might be solved by the **git pull -r**

this command is used to pull the change from the remote server, and rebase the head. the GIT will do 
merge automatically.

### git Create new branches
git checkout -b BRANCHNAME
