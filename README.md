
Putting it on your local machine will make it  easier to work with. 
## Cloning:
   the process of copying the repository from GitHub to your local machine (sometimes referred to as "checking out"
    - Pulling: down a full copy of all the repository data that GitHub has at that point in time to include all versions of every file and folder for the project
	- Pushing: you can push your changes to the remote repository on GitHub or pull other peoples changes for GitHub
Pushing Commits to a remote repository: use git push to push commits made on your local branch to a remote repository

	1. Navigate to the main page of the repository 
	2. Above the list of files click CODE
	3. To clone the repo using HTTPS, under "Clone with HTTPS" click copy, to clone the repo using an SSH key, including a certificate issued by your organizations SSH certificate authority, click use SSH then click share
	4. Open Terminal
	5. Change the directory to the location where you want the cloned directory
	6. Type git clone and then past the URL you copied earlier 
	7. $ git clone 

## Changing the user Issues
	- Git config credential.username 'github name' 
	- Pull the information
		○ Git pull origin master 
	- Push the files back 
		○ Git push -f origin master 
## Pushing files to an existing repo on Github
	1. Open terminal
	2. Change the current directory to your local project 
		○ My directory is ~/documents/Assignment2/Assignment2 
	3. Initialize the local directory as a Git repository 
		○ Git init 
	4. Add the files in your new local repo. This stages them for the first commit 
		○ Git add . 
			§ Adds the files in the local repo and stages them for commit
	5. Commit the files you've staged in your local repo
		- Git commit -m "First commit"
			§ Comits the tracked changes the prepares them to be pushed to a remote repo
	6. Copy the remote repo URL
	7. Add the URL for the remote repo where your local repo will be pushed 
		- Git remote add origin 'repo URL name'
			§ Sets the new remote
		- Git remote - v
			§ Verifies the new remote url
	8. Push the changes in your local repo in your local repo to Github
		- Git push -u origin master 
Pushes the changes in your local repo up to the remote repo you specified as the origin
