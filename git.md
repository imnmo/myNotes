#git

a good reference for git of course is http://git.scm

### preparing for review
as usual with ...

* git add <file>
* git commit
* 

### First time pushing for review 
* git push review

### On Squashing 

* *git rebase -i HEAD~2*
	* *pick* old patch set abd *squash* latest one. 
	* A new editor pops up, delete the 2nd commit message 

### In case of commit is lost, with Squash
* If the commit is lost	
	* git reflog
	* git reset --hard bcfb0a5(your commit level)
	* Follow your steps

### renaming files and directory 

To rename files or directories the following steps needs to be followed:

* git mv or mv oldfolder/oldfile newfolder/newfile
	* try to always us mv ## since git mv tries to append the stuff

## Deleting any recursive folder 
* git rm -r oldfolder
* git commit
* git push review


## Update your local(master) branch to origin/master:
* DO's:
	* git rebase origin/master
	* git mergetool (in case of merge conflict, use mergetool and fix the changes)
	* git rebase -- continue
* DONT'S:
	* don't do git pull on your local(master)
	* not required to do git commit after fixing your merge conflicts while doing git rebase