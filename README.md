# Hello-World
This is my very first repository on GIthub. 

##### Subheader

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

Next step is to learn how to create a repository localy and then push it onto github.
- Create a folder/repo locally
- Create files inside this repo
- use the command "git init" to make the repo into a github repo. But note that this repo is still not on github 
- Then go to github and create an empty repo with the same name as the local repo
- Copy the ssh code given 
- Then use the command git remote add origin ssh-code
- Then commit and push files as usual
