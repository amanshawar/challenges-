- [ ] **Why do we use github/git?**

It lets you and others work together on projects from anywhere by storing remote copies of your 
projects/repositories (github servers) as backup of your local copies.

- [ ] **What happens when you clone a repository?**

You can clone your repository to create a local copy on your computer and sync between the two 
locations.

- [ ] **What happens when you fork a repository?**

A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes 
without affecting the original project. Most commonly,forks are used to either propose changes to 
someone else's project or to use someone else's project as a starting point for your own idea

- [ ] **What happens when we do git pull origin master**

 git pull origin master pulls the master branch from the remote called origin into your current branch.
 
- [ ] **How do we create a new branch on our local machine?**

git checkout branchName

- [ ] **When we make a change to a file, how do we tell git to track it?**

git add fileName

- [ ] **When we have finished working on a branch, how do we make sure that**
**our changes do not cause a conflict with master? (this can all be done locally)**

on branch
git add filesName
git commit -m "M"
git checkout master
git pull origin master
git checkout branch
git merge master

if there is conflicts will be appear,then solve conflicts.

- [ ] **What does git push origin [branch-name] do?**

push the changes on this branch from local to remote github 

- [ ] **Why do we make pull requests instead of just changing master directly?**

to make sure there is no conflicts
to show the changes to others in the team and make approve to it 

- [ ] **Why is it important to run our team member’s branches when they make a pull request?**

to make sure the braanch work and will not crash all the work on master

This is the working process you should follow, try to explain what happens at each step/why we do it:

git clone [repository]

git checkout -b new-feature

make some changes to index.js

git add index.js

git commit -m "added a cool new feature"

since we started, our partner has merged another branch into master

git checkout master

git pull origin master

git checkout new-feature

git merge master

merge conflict happens in index.js we fix it

git add index.js

git commit -m "fix merge conflict"

git push origin new-feature
