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




## Branches

- 'git branch <NAME> ': create branch <NAME> where you are (Head)
- 'git switch <NAME> ': move to the branch <NAME> 
	-'git checkout <NAME> ': also move to the branch <NAME>
- 'git switch -c <NAME> ' : create and move to the branch <NAME>
	- 'git checkout -b <NAME> ': same thing as above 
- 'git merge <BRANCH> ': merge <BRANCH> into your current branch

- 'git rebase ' : command to change the history of a commit
	- 	- Commits from 'git merge' can be automatically combined 
-'git rebase <BRANCH> ': incoporate  changes from <BRANCH> into current branch
	- 'git status': is your friend 
	- 'git add <FILE>': to mark conflict resolution
	- 'git rebase --continue': move to next commit in rebase
	- 'git rebase --abort' : undo git rebase step 

- 'git rebase -i <COMMIT>' 'HEAD~' or <HASH> of commit to go into interactive rebase
	- you can make multiple commit change here, e.g, 'squash'/'s'
	- 'git rebase -i <HASH>^': use ^ to include that commit in interactive rebase
- 'git stash' or 'git commit': to save work before moving branches
	- 'stash' is temporary
	- 'git stash list': see your stashed commits
	- 'git stash clear': clean up your stashes
- A `merge` on the remote is called a "pull request" or "merge request"
	- `git push <WHERE> <WANT> `
	- to update a PR, we make changes to the branch locally and re "push" 
