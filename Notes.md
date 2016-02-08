##UDACITY - GITHUB##

###Lessons 1 & 2 - WOrking with Git

Config:
- `git config --global color.ui auto` to configure colour output
- `git config --global credential.helper wincred` to cache credentials

Commands:

- `git diff commit1 commit2` shows the changes from `commit1` to `commit2`
	- `git diff` naked shows diff of cwd to parent
	- `git diff --staged` to show the diff of staging directory to parent
- `git log` shows the commit history starting with the most recent
	- `git log --oneline` shows a shortened view
	- `git log --graph --oneline` shows a compact treeview of the commits along the current branch
- `git clone source` copies `source` repo to current working directory
- `git commit` starts the commit process
- `git checkout branch/commit` changes files to match to tip of `branch` or as at `commit`
- `git init` creates a new repository in the current working directory
	- `git init sub_dir` will create a repo in new dir `sub_dir` of cwd
- `git status` shows the state of the staging area (things added but not yet committed)
- `git reset --hard` resets working directory to the staging dir
- `git branch` will show list of branches, with currently checked out branch starred (if applicable)
	- `git branch new_name` creates a new named branch
	- `git checkout -b new_branch_name` provides a shortcut to create & move to a new named branch. Equivalent to running:
		- `git branch new_branch_name` to create the new branch
		- `git checkout new_branch_name` to switch to the newly created branch
- `git merge branch_name` will begin a merge of `branch_name` branch into the currently checked out branch
	- **Note**: When there are conflicts via command line, open the file to edit and resolve. Looks for `<<<<<<` and `>>>>>>` markers.
- `git show [commit_id]` shows the diff of `commit_id` from its *parent*
	- without a parameter, the command will show the diff of the most recent commit from its parent

###Lesson 3 - Working with GitHub

Create a new repository on GitHub. Only use the initialize with README option if you do not have a repo with files already set up locally (ie, only when starting fresh).

- `git remote` lists current remotes
- `git remote add remote_name remote_url` sets up a new remote. Using `origin` is standard as a name when you will only have a single remote.
	- eg: `git remote add origin https://github.com/BrendanFDMoore/udacity-git.git`




##Asteroids##

Repository Diagram:
										  /--Easy Mode----/--Easy mode--
	Master (revert controls)--v- Master -^------Master---^-----Master--
                              V-- Coins ----^

