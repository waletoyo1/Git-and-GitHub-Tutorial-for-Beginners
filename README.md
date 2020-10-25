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
          <p>  a. <b>git init</b> then press enter</p>
          <p>  b. <b>git config user.name yourName</b> then press enter</p>
           <p> c. <b>git config user.email yourEmail</b> then press enter.</p> NB: If you have a GitHub account, make sure your git email corresponds to your GitHub email as this helps your contributions to reflect on your profile.
    



# 3. Stages in Vesion controlling using Git (Modify, Stage, & Commit)
<p>a. Modify - This involve changing and saving your codes.</P>
<p>b. Stage - Before a modified code can be tracked or commited, it has to be stagged. Use the following commands to stage your codes:</P>
  <p><b>git add fileNmae</b>  or <b>git add . </b>  (to stage more than one file).</P>
 <p> <b>git status</b>  (to check if your files has been staged).</p>
<p>c. Commit - This is done after stagging your codes. At this point seem satisfied with what you have written and want it to be trackable. Use the following commands for commiting your codes: 
  <b>git commit -m "commit name" </b> then press enter. NB: Commit name helps you to remember what that code is all about. E.g "added index.html"
  <b>git log</b> (to view your commit history)
  <b>git log --oneline</b> (to view your commit history in one line).</P>
  
  
  
# 4.  Git Undoings (Checkout, Revert & Reset)
 <p> <b>Checkout</b> - helps to navigate from one commit to another in a particular code branch. Use the following commands to checkout or navigate your commits or branch</P>
 
    <p> <b>git checkout commitID</b>  (NB: commitID can be obtained when you check your commit history)</P>
   <P> <b>git checkout master</b> (to navigate to the master branch)</P>
  <p> <b> git checkout branchName</b> (to naviage to another branch other than the master branch).</p>
    
<p> <b>  Revert</b> - helps to create another commit after modifying a particular commit of a particular branch. For example, you have a commit called "hello world" containing "<p>Hello world</p>" as the content. If want to change the content to <p> Hello Nigeria </p>, you need to make another commit by reverting the "hello world" commit. This preserves the "hello world" commit and also produce a new commit e.g "Hello Nigeria".  Use the steps below for reverting your commit:</p>
    <p>1. Stage your code by entering <b>git add .</b> </P>
  <p>  2. Revert your commit by entering <b>git revert newCommitName</b> then press enter</P>
 
<p> <b> Reset</b> - When you reset a commit, all the commit history before it will be deleted. Lets assume we have the following commits a->b->c->d->e->f. When we reset our commit history to e, commits a,b,c and d will be deleted. Use the command below to reset to a commit:
   <b> git reset desiredCommitID --hard</b></p>
    
 
 

  
 # 4.  Branching
  Branching helps to introduce new fetures to your app without affecting the master branch. NB: The master branch is the stable version of your app and its the repository or folder that was created when git is initiated.
  To create a new barnch, use the following commands:
   <b>git branch branchName</b>
   NB: You have to checkout your new branch before you can stage or make commits in it. Use git checkout branchName
   Use <b>git checkout -b branchName</b> to create and checkout a new branch simultaneously.
  





