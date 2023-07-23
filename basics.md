### upstream & downstream in git: 
upstream is from where you clone your repository and downstream is one cloned by the upstream ,which will be pushed. 
### git blame: 
git blame Shows what revision and author last modified each line of a file.  https://www.git-scm.com/docs/git-blame
### git lense: 
Part of GitKraken's legendary **Git tools** ,lense helps in PR review.  https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens

### git log: 
To check PR author ,co-authors ,merge date , merge ID 

### git log --graph --format=format:’<>’ --all : 
To see all the logs of git log with all merge commits with branch tree
--graph adds a tree graph on left. 
--Format: To customize your preset logs. There are preset formats to choose and can be customized too. For preset formats: https://git-scm.com/docs/git-log#_commit_formatting.
--all: includes all of the refs, tags, branches in the logs. If donot want all info use preset commands from: https://git-scm.com/docs/git-log#Documentation/git-log.txt---all.

### git show:-------- 
Can show high-level view of changes. 
### git show <commit> --stat: 
<commmit> is the commit id and ,
--stat: To see the commit summary and the changes files.

### git show <commit> filepath : 
This gives specific file line changes for your file. 

### git merge vs git rebase: 
When there are changes in the main branch and you want the same in your branch, you can do git rebase or merge.
merge takes the changes from one branch and merges them into another branch in one merge commit. 
```
git merge origin/main your-branch
```
git rebase moves the branch to a new starting point from the base branch. 
```
git rebase origin/main your-branch
```
Generally, you’ll use rebase when there are changes in an upstream branch (like main) that you want to include in your branch. You’ll use merge when there are changes in a branch that you want to put back into main.

### git squash : 
It is used to combine multiple commits into one. It is mostly used to combine multiple multiple branches. 
By default, a pull request (PR) will be a merge commit, so after the PR is merged, the entire history of the working branch will be merged in, plus an additional merge commit. you can set your repository to “squash and merge” by default, meaning merged PRs will result in only a single commit each, instead of bringing over all the commits from the working branch to keep the merge history clean. 
squash commits loses information and causes to rework as a bug. 

