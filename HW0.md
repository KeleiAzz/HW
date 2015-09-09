##Git commands:

###Introduction Sequence


Level 1

	git commit -m "c1"
	git commit -m "c2"
	
Level 2

	git branch bugFix
	git checkout bugFix
	
Level 3

	git branch bugFix
	git checkout bugFix
	git commit -m "c1"
	git checkout master
	git commit -m "c1"
	git merge bugFix
	
Level 4
	
	git branch bugFix
	git checkout bugFix
	git commit -m "c1"
	git checkout master
	git commit -m "c1"
	git checkout bugFix
	git rebase master
	
###Ramping Up

Level 1
	
	git checkout C4
	
Level 2
	
	git checkout bugFix^
	
Level 3
	
	git branch -f master C6
	git branch -f bugFix HEAD~2
	git checkout C1
	
Level 4

	git checkout pushed
	git revert HEAD
	git branch -f local HEAD~2
###Screenshot

![image](https://github.ncsu.edu/raw/kgong/DevOps-HW/master/Screenshot%202015-09-08%2019.43.18.png?token=AAALM1qYkpEf7T3u6N9S3fFBxhk19cv8ks5V-LbswA%3D%3D)

###Content in post-commit

	\#!/bin/bash
	open http://www.ncsu.edu

And run this command:

	chmod +x .git/hooks/post-commit
	
[Screencast](https://drive.google.com/a/ncsu.edu/file/d/0B87f7178bIHnaXJKems5Wm5KT3M/view?usp=sharing)

