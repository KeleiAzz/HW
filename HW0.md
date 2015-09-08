Introduction Sequence

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
	
Ramping Up

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