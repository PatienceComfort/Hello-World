# Hello-World
This is my very first repository on Github. I'll be using it to learn git (in addition to getting the handle of visual code)
I'll also be using atlassian's git guide as a cross-reference for the youtube tutorial I'm following
Atlassain : https://www.atlassian.com/fr/git/tutorials
Youtube : https://www.youtube.com/watch?v=RGOj5yH7evk&list=PL7ZPz7ipvBRbmjpnLp-FhlqR4m39WMkcH&index=79&t=38s&ab_channel=freeCodeCamp.org


## Cloning and updating a repo

Modifying a repo from github:
First step: cloning
use the command "git clone repo-ssh-adress"
You can then move into the files (by clicking or by cd) and modify them. You can also create new files.  Once that is done, you can then push the changes onto github with commands that must be in the correct order
Correct order:
- git status
- git add .
- git status (to check if the changes have been tracked)
- git commit -m "Message title" -m "Message text"
- git push / git push origin master

I still dont understand what "git push origin master" is meant for. When I enter this command, It tells me that "Everything is up-to-date" but it doesn't push any of the chages onto my online repo. Unless I go through the regular status, add, commit first. So basically does the same thing as "git push"

## Creating a repo locally 
Next step is to learn how to create a repository localy and then push it onto github.
- Create a folder/repo locally
- Create files inside this repo
- use the command "git init" to make the repo into a github repo. But note that this repo is still not on github 
- Then go to github and create an empty repo with the same name as the local repo
- Copy the ssh code given 
- Then use the command git remote add origin ssh-code
- Then commit and push files as usual

## Branching 
The master branch is the main/default branch. Unless you create another branch, all your code and changes will be on the master branch.
When you make another branch (feature branch), at first, the code within the two branches will be exactly the same. But as you make changes, the changes will only appear in the feature branch. This allows our code to be tested without corrupting the main code. 
And in case you make multiple branches, each branch has no way of knowing what was commited onto the other branches.

So how do I create a new branch locally?
- First check what branch you are operating on with "git branch". It should show you all the branches you have and indicate which branch you are on with a star 
- Then you run the command "git checkout -b branchName" to create a new branch and "git checkout branchName" to switch to an already existing branch
- To set up the brach upstream (online), once you've added and commited your changes in your branch, you use the commande "git push --set-upstream origin branchName" or "git push -u origin branchName"

Ways to merge branch with master 
- Check the differences by going back into master then the command "git diff branchName"
- With the command "git merge branchName"
- With a pull request (on the github page)
Once the pull request is done, anyone can review our code and decide to merge it with the master 

Once you're done with your feature branch (once the merging is done) it's best practice to delete the branch. That can be done with the command "git branch -d branchName"

## Dealing with merge conflicts 


