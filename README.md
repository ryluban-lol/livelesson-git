- 'git init': initialize current folder as a git repository
- 'git clone <URL>': brings the git repo from <URL> to current folder
- 'git status' : tells us what we need to know about our repository

- 'git add <File>' : adds <FILE> to the staging area
- 'git commit ': opens a text editor to write commit message 
	- 'git commit -m "MESSAGE" ' : writes MESSAGE as a commit without a text editor
- 'git log' : shows the history o four commits
	- 'git log --oneline': shows the shorter oneline commit 
- 'git diff': compare current uncommited state with last known git state
	- 'git diff --staged' : runs git diff between the staging area and last known state
- ' git diff HEAD~<NUMBER> ': compares HEAd with commit <NUMBER> ago (relative)
- 'git diff <HASH>: compares HEAD with the commit in <HASH>

-'git restore -- source <HASH OR HEAD~> <File> ': restore file to <HASH OR HEAD>
		- 'git checkout <HASH OR HEAD~> <FILE> ': restores file to <HASH or HEAD~>
		- 'git checkout master': go back to master
		- 'git switch master': go back to master
