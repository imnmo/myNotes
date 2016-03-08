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

* git mv oldfolder/oldfile newfolder/newfile
* git add newfolder
* git rm -r oldfolder
* git commit
* git push review