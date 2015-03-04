# Git

## Git 常用指令

* Status

	* Show Status
	
	```` Command
	CLOUD-33:BasicGit cookie$ git status
	On branch master
	Your branch is up-to-date with 'origin/master'.
	nothing to commit, working directory clean
	````

* Branch

	* Show Local Branch List

	``` Command
	CLOUD-33:BasicGit cookie$ git branch
	* master
	```
	
	* Show All Branch List
	
	* Create Branch
	
	```` Command
	CLOUD-33:BasicGit cookie$ git branch issue-somthing
	CLOUD-33:BasicGit cookie$ git branch
	  issue-somthing
	* master
	````
	
	* Change Branch
	
	```` Command
	CLOUD-33:BasicGit cookie$ git checkout issue-somthing
	Switched to branch 'issue-somthing'
	CLOUD-33:BasicGit cookie$ git branch
	* issue-somthing
	  master
	````

* Add 

	* Add one file
	
	```` Command
	CLOUD-33:BasicGit cookie$ git status
	On branch issue-somthing
	Changes not staged for commit:
	  (use "git add <file>..." to update what will be committed)
	  (use "git checkout -- <file>..." to discard changes in working directory)

		modified:   markdown/GitCommand.md

	Untracked files:
	  (use "git add <file>..." to include in what will be committed)

		test/
		tmp.txt

	no changes added to commit (use "git add" and/or "git commit -a")
	CLOUD-33:BasicGit cookie$ git add test
	CLOUD-33:BasicGit cookie$ git status
	On branch issue-somthing
	Changes to be committed:
	  (use "git reset HEAD <file>..." to unstage)

		new file:   test/aaa.tt
		new file:   test/tmp.txt

	Changes not staged for commit:
	  (use "git add <file>..." to update what will be committed)
	  (use "git checkout -- <file>..." to discard changes in working directory)

		modified:   markdown/GitCommand.md

	Untracked files:
	  (use "git add <file>..." to include in what will be committed)

		tmp.txt
	
	````
	
	* Add All files
	
	```` Command
	CLOUD-33:BasicGit cookie$ git status
	On branch issue-somthing
	Changes to be committed:
	  (use "git reset HEAD <file>..." to unstage)

		new file:   test/aaa.tt
		new file:   test/tmp.txt

	Changes not staged for commit:
	  (use "git add <file>..." to update what will be committed)
	  (use "git checkout -- <file>..." to discard changes in working directory)

		modified:   markdown/GitCommand.md

	Untracked files:
	  (use "git add <file>..." to include in what will be committed)

		tmp.txt

	CLOUD-33:BasicGit cookie$ git add .
	CLOUD-33:BasicGit cookie$ git status
	On branch issue-somthing
	Changes to be committed:
	  (use "git reset HEAD <file>..." to unstage)

		modified:   markdown/GitCommand.md
		new file:   test/aaa.tt
		new file:   test/tmp.txt
		new file:   tmp.txt
	````
