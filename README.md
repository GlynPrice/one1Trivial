#one1Trivial

##git status Command
The `git status` command, I believe, **only** displays changes/work for the local git repository. It gives **no** information about the need or otherwise to:  
1. update (i.e. download) (synchromise with changes/work of other remote users) files/subfolders **from** the associated remote git repository
2. update (i.e. upload) (archive the local changes/work) files/subfolders **to** the associated remote git repository.  

The following sequence of git online commands (Terminal window) might be useful to establish the current status of the local git repository.  
```
ls -la
git status
git add .
git status
git commit -m "comment"
git status
git rmote -v
```
The above set of commands with `add` and `commit `ensure that the local changes, if any, are known to the local git repository. So when the following `pull` and `push` are done then then any need to merge changes/work are with respect to the local repository including all work/changes. Otherwise the changes/work will be overwritten.

git pull origin master				Already up-to-date
git push origin master #Everything up-to-date

