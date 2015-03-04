# Git

## Git 常用指令

* Status

``` Command
CLOUD-33:BasicGit cookie$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
nothing to commit, working directory clean
```

* Branch
	* Local Branch List

	``` Command
	CLOUD-33:BasicGit cookie$ git branch
	* master
	```
	
	* All Branch List
	
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
