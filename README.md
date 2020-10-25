# Git-and-GitHub-Tutorial-for-Beginners
This tutorial explains the basics of Git and GitHub

# TABLE OF CONTENTS

1. Introduction to Git
2. Installing Git
3. Stages in Vesion controlling using Git (Modify, Stage, & Commit)
4. Git Undoings (Checkout, Revert & Reset)
5. Branching
6. Merging Branches
7. Introduction to GitHub
8. Pushing (local to remote)
9. GitHub Alias
10. Pulling or Cloning ( remote to local)
11. Collaborating on GitHub (privately and publicly)



# 1. Introduction to Git
Git is a software for tracking versions of your codes during software development.



# 2. Installing Git
  - Vist https://git-scm.com/download/win for Windows PC and https://git-scm.com/download/mac for Mac PC.
  - Follow the instructions and install.
  - After the installation is completed, go to your project directory and open your command line terminal using that path.
  - Configure your using the following commands:
    a. "git init" the press enter
    b. "git config user.name yourName" then press enter
    c. "git config user.email yourEmail" then press enter. NB: If you have a GitHub account, make sure your git email corresponds to your GitHub email as this helps your contributions to reflect on your profile.
    



# 3. Stages in Vesion controlling using Git (Modify, Stage, & Commit)
a. Modify - This involve changing and saving your codes.
b. Stage - Before a modified code can be tracked or commited, it has to be stagged. Use the following commands to stage your codes:
  git add fileNmae  or git add .   (to stage more than one file).
  git status  (to check if your files has been staged).
c. Commit - This is done after stagging your codes. At this point seem satisfied with what you have written and want it to be trackable. Use the following commands for commiting your codes: 
  git commit -m "commit name" then press enter. NB: Commit name helps you to remember what that code is all about. E.g "added index.html"
  git log (to view your commit history)
  git log --oneline (to view your commit history in one line).
  
  
  
# 3.  Git Undoings (Checkout, Revert & Reset)
  Checkout - helps to navigate from one commit to another in a particular code branch. Use the following commands to checkout or navigate your commits or branch
    git checkout commitID  (NB: commitID can be obtained when you check your commit history)
    git checkout master (to navigate to the master branch)
    git checkout branchName (to naviage to another branch other than the master branch).
    
  Revert - helps to create another commit after modifying a particular commit of a particular branch. For example, you have a commit called "hello world" containing <p>Hello world</p> as the content. If want to change the content to <p> Hello Nigeria </p>, you need to make another commit by reverting the "hello world" commit. This preserves the "hello world" commit and also produce a new commit e.g "Hello Nigeria".  Use the steps below for reverting your commit:
  
  





