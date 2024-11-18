task list1
Added a discription
# Task 1 : Install and Configure Git
## 1.Configure Git with your username and email
git config --global user.name "Your Name"
-->define username
git config --global user.email "krihshyara25@gmail.com"
-->define useremail

## 2.View your Git configuration:
git config --list
-->view your configuration

# Task 2 : Initialize a Repository:
## 1.Create a new project folder and navigate to it:
mkdir MyProject
-->make a folder named MyProject

cd MyProject
-->enter in MyProject

## 2.Initialize it as a Git repository:
git init 
-->initialize git repo.

# Task 3 : Create a File and Make Multiple Commits
## 1.Create a new file and add content:
echo "My First Project" > README.md
-->create a file named README.md and add text in it

## 2.Stage the file:
git add README.md
--> add changes to staging to the area

## 3.Commit the file:
git commit -m "Initial commit: Added README.md"
-->give a commit message 

## 4.Make changes to the file:
echo "Added a description" >> README.md
-->Added some text in file

## 5.Stage and commit the changes:
git add README.md
git commit -m "Updated README with a description"
-->add readme.md file to staging area and give a commit message to it.

# Task 4:Check Status and log
## 1.Check the repository's current status:
git status
-->Give the details of the current state of your staging area

## 2.View commit history in detail:
git log --oneline --graph --decorate
--> Give the details of every commits 

# Task 5:Create and Clone a Repository
## 1.Create a repository on GitHub named example-repo.
## 2.Clone it locally:
git clone http://codinggita.com/example-repo
-->clone the repo. in your local storage

# Task 6: Understanding the Git Workflow
## 1.Make changes to a file in the working directory:
echo "Workflow example" > workflow.md
-->create a file named workflow.md and add some text
## 2.Stage the file:
git add workflow.md
-->Add file to staging area
## 3.Commit the file to the repository:
git commit -m "Added workflow example"
-->give a commit message to the file

# Task 7:Branching and Merging
## 1.Create a new branch for a feature
git branch feature-login
-->create a new branch named feature-logic

git checkout feature-login
-->open in feature-logic branch

## 2.Add a new file and commit changes:
echo "Login Page" > login.html
-->craete a file named logic.html

git add login.html
-->add file to staging area

git commit -m "Added login page"
-->give a commit message

## 3.Merge the feature branch into main:
git checkout main
-->switch to main branch

git merge feature-login
-->merge main branch to feature-login branch

# Task 8: Handling Merge Conflicts
## 1.Create two branches:
git branch branch-A
-->create branch named branch-A

git branch branch-B
-->create branch named branch-B

## 2.Modify the same line in README.md in both branches.
-->checkout both branches and add some text in README.md file
-->then add and commit files

## 3.Merge branch-A into main:
git checkout main
-->switch to main branch

git merge branch-A
-->merge branch A and main

## 4.Attempt to merge branch-B into main (this will cause a conflict):
git merge branch-B
-->merge branch B and main

## 5.Resolve the conflict manually in README.md, then:
git add README.md
git commit -m "Resolved merge conflict between branch-A and branch-B"
-->add README.md file and give a commit message

# Task 9:Renaming and Deleting Branches
## 1.Rename a branch:
git branch -m old-branch-name new-branch-name
-->change the name of the branch

## 2.Delete a branch:
git branch -d feature-login

# Task 10:Using Git Stash
## 1.Make changes to a file but don’t commit:
echo "Temporary work" >> temp.md
-->add text in file 

## 2.Stash the chnages
git stash
-->temporarily saving uncommitted changes

## 3.View stashed changes:
git stash list
-->list of all stashes

## 4.Apply the stashed changes:
git stash apply
-->changes the stashes that are given before

## 5.Drop the slash after applying:
git stash drop
-->remove a specific stash entry from the stash list

# Task 11: Rewriting History with Interactive Rebase
## 1.Create multiple commits:
echo "Commit 1" > file1.txt && git add file1.txt && git commit -m "Commit 1"
echo "Commit 2" > file2.txt && git add file2.txt && git commit -m "Commit 2"
echo "Commit 3" > file3.txt && git add file3.txt && git commit -m "Commit 3"
-->create , add and commit many files

## 2.Squash commits into one:
git rebase -i HEAD~3
-->

# Task 12:Cherry-Picking Commits
## 1.Create a new branch:
git checkout -b cherry-pick-example
-->create a new branch named cherry-pick-example

## 2.Cherry-pick a specific commit from another branch:
git cherry-pick <commit-hash>
-->to copy the commit in another branch

# Task 13:Tagging commits
## 1.Tag the current commits:
git tag -a v1.0 -m "Version 1.0 release"
-->Create an annotated tag for a release
-->Annotated tags are generally recommended for marking releases.

## 2.Push the tag to the remote repository:
git push origin v1.0
-->push a specific tag

# Task 14:Working with Remote Repositories
## 1.Add a Remote Repository:
git remote add origin <repository-url>
-->add a new repository to your local repository

## 2.Push your changes to the remote repository:
git push origin main
-->to push your local changes from main to remote Repository

# Task 15:Forking and Contributing
## 1.Fork a repository on Github.
-->click the fork icon in git repository

## 2.Clone the fork locally:
git clone <forked-repo-url>
-->clone the repository to store in local storage

## 3.Create a new branch, make changes, and push:
git checkout -b fix-typo
echo "Typo fixed" >> README.md
git add README.md
git commit -m "Fixed a typo"
git push origin fix-typo
-->switch to fix-typo branch , add text in README.md file , add README.md file to staging area , give a commit message to file , push to fix-typo branch

## 4.Open a pull request on GitHub.
--> send a pull request to repository

# Task 16:Simulate Team Collaboration
## 1.Create a repository and share it with a friend.
## 2.Both make changes to the same file simultaneously.
## 3.Practice resolving merge conflicts and pushing changes.

# Task 17:Git Ignore
## 1.Create a .gitignore file:
echo "node_modules/" > .gitignore
-->create a file with .gitignore formate

## 2.Add files and ensure ignored files are not staged:
git add .
--> add all files to staging area
