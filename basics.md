### git log: 
To check PR author ,co-authors ,merge date , merge ID 

### git log --graph --format=format:’<>’ --all : 
To see all the logs of git log with all merge commits with branch tree
--graph adds a tree graph on left. 
--Format: To costomize your preset logs. There are preset formats to choose and can be customized too. For preset formats: https://git-scm.com/docs/git-log#_commit_formatting.
--all: includes all of the refs, tags, branches in the logs. If donot want all info use preset commands from: https://git-scm.com/docs/git-log#Documentation/git-log.txt---all.

### git show:-------- 
Can show high level view of changes. 
### git show <commit> --stat: 
<commmit> is the commit id and ,
--stat: To see the commit summary and the changes files.

### git show <commit> filepath : 
This gives specific file line changes for your file. 
