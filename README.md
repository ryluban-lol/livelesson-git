# Git Notes
## Working with git locally
'git init': initialize current folder as a git repository

'git clone ': brings the git repo from to current folder

'git status' : tells us what we need to know about our repository

'git add ' : adds to the staging area

'git commit ': opens a text editor to write commit message

'git commit -m "MESSAGE" ' : writes MESSAGE as a commit without a text editor
'git log' : shows the history o four commits

'git log --oneline': shows the shorter oneline commit
'git diff': compare current uncommited state with last known git state

'git diff --staged' : runs git diff between the staging area and last known state
' git diff HEAD~ ': compares HEAd with commit ago (relative)

'git diff : compares HEAD with the commit in

-'git restore -- source <HASH OR HEAD~> ': restore file to - 'git checkout <HASH OR HEAD~> ': restores file to <HASH or HEAD~> - 'git checkout master': go back to master - 'git switch master': go back to master

## Working with remotes
'git remote add ': adds the as a remote with the name - is by convention called 'origin'
'git remote -v': look at all the remotes you have
'git push ': pushes the branch to - 'git push origin main'
'git remote rm ': removes the remote called
'git pull ': pulls the branch in to local computer


## BRANCHES - main commit 3

- 'git branch <NAME> ': create branch <NAME> where you are (Head)
- 'git switch <NAME> ': move to the branch <NAME> 
	-'git checkout <NAME> ': also move to the branch <NAME>
- 'git switch -c <NAME> ' : create and move to the branch <NAME>
	- 'git checkout -b <NAME> ': same thing as above 
- 'git merge <BRANCH> ': merge <BRANCH> into your current branch

- 'git rebase ' : command to change the history of a commit
	- 	- Commits from 'git merge' can be automatically combined 
-'git rebase <BRANCH> ': incoporate  changes from <BRANCH> into current branch

- main commit 1
- main commit 2
