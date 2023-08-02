Version-Control:

Initialize a New Repository (git init):

Initialize a new Git repository in the current directory: git init

Clone a Repository (git clone):

Clone a remote repository to the local machine: git clone remote_repository_url
Example: git clone https://github.com/user/repo.git

Add and Commit Changes (git add and git commit):

Add changes to the staging area: git add file1 file2
Commit the changes with a message: git commit -m "Commit message"

View Repository Status (git status):

View the status of files in the repository: git status

View Commit History (git log):

View the commit history with detailed information: git log
View a compact commit history: git log --oneline

Create and Switch Branches (git branch and git checkout):

Create a new branch: git branch new_branch_name
Switch to an existing branch: git checkout branch_name
Create and switch to a new branch: git checkout -b new_branch_name

Merge Branches (git merge):

Merge a branch into the current branch: git merge branch_name

Pull and Push Changes (git pull and git push):

Pull changes from the remote repository: git pull origin branch_name
Push local changes to the remote repository: git push origin branch_name

View Remote Information (git remote):

View a list of remote repositories: git remote -v

Discard Changes (git restore):

Discard changes in the working directory: git restore file_name

Stash Changes (git stash):
Temporarily save changes to the stash: git stash
Apply stashed changes to the current branch: git stash apply

		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these Version Control commands with Git:
		
		Initialize a New Repository (git init):
		
		git init: Initializes a new Git repository in the current directory.
		
		Clone a Repository (git clone):
		
		git clone https://github.com/user/repo.git: Clones the remote repository from GitHub to the local machine.
		
		Add and Commit Changes (git add and git commit):
		
		git add file1 file2: Adds changes in file1 and file2 to the staging area.
		git commit -m "Initial commit": Commits the changes with the message "Initial commit."
		
		View Repository Status (git status):
		
		git status: Displays the status of files in the repository.
		
		View Commit History (git log):
		
		git log: Shows the detailed commit history.
		git log --oneline: Displays a compact commit history with one-line information per commit.
		
		Create and Switch Branches (git branch and git checkout):
		
		git branch feature_branch: Creates a new branch named feature_branch.
		git checkout feature_branch: Switches to the feature_branch.
		
		Merge Branches (git merge):
		
		git merge feature_branch: Merges the changes from feature_branch into the current branch.
		
		Pull and Push Changes (git pull and git push):
		
		git pull origin main: Pulls changes from the main branch of the remote repository.
		git push origin feature_branch: Pushes local changes to the feature_branch of the remote repository.
		
		View Remote Information (git remote):
		
		git remote -v: Displays a list of remote repositories and their URLs.
		
		Discard Changes (git restore):
		
		git restore file_name: Discards changes in the file_name in the working directory.
		
		Stash Changes (git stash):
		
		git stash: Temporarily saves changes to the stash.
		
		These Git commands are fundamental for version control and collaboration in software development. They help developers manage changes, work with branches, and synchronize code with remote repositories effectively. Remember to adjust the command examples according to your specific Git repository and workflow.