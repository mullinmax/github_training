# Github tutorial
### *A repo designed for teaching Git and Github*
#### How to get started:

- Install Git
	- windows:
		- [download](https://git-scm.com/download/win) and install git for windows.
		- **(optional)** [download and install cmdr](http://cmder.net/)
	- Linux/OSX:
		- if you don't already have git installed type:
	
    		`sudo apt-get install git`
 - Clone this repository
 	- Open GitBash on windows or your terminal on linux/OSX
 	- Navigate to a folder where you would like to keep your local copy of the repo and run `git clone https://github.com/mullinmax/github_tutorial.git`
 	- You will be required to sign in with your github username and password, In the future you [can avoid this using SSH keys](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/).
 - Make an edit
 	- Before we can do anything we need to make a branch we can work in without disturbing anyone else while they waork. type `git branch myNewBranch` make sure to change *myNewBranch* to something new. Once a branch has been created and added to the repository another cannot share the same name.
 	- Switch to the new branch by running `git checkout myNewBranch`
 		- **(bounus)** you can do both commands in one by running `git checkout -b myNewBranch`
 	- Find R_and_J.txt in your newly cloned repository and open it with your favorite editor.
 	- scroll down a bit and make any change to the file and save it.
 - Upload an edit
 	- Back in the terminal type `git add R_and_J.txt`this says to git that `R_and_J.txt` is going to be in the next commit.
 	- Now type `git status` you should see just `R_and_J.txt` listed as *staged for commit*. If you see anything different, you probably changed something else or didn't save your changes to `R_and_J.txt` 
 	- If `git status` returned good results. type `git commit -m "I made a change to R_and_J.txt and it was awesome"` with your own message. This message is what other collaborators will see on git hub with your changes. Try to keep them breif and descriptive.
 	- Run `git push`. If this is your 1st time pushing from a particular computer, repository, or branch git will ask you to run some simple commands with information like your email or name. This is so collaborators can contact you about the changes you made in the future.
- Merge your changes
	- Merging is a little different in every team, some require a peer reveiw(s), some have no restrictions, some are flexible. Github has some flexible settings that allow you to setup a repo to enforce many common rules on merging.
	- to merge a branch simply run `git checkout branchYouAreMergeingINTO`
	- then `git merge incomingBranch`
