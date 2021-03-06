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
  - After the installation is completed, go to your project directory(repository) and open your command line terminal using that path.
  - Configure your  repository for Git using the following commands:
          <p>  a. <b>git init</b> then press enter</p>
          <p>  b. <b>git config user.name yourName</b> then press enter</p>
           <p> c. <b>git config user.email yourEmail</b> then press enter.</p> NB: If you have a GitHub account, make sure your git email corresponds to your GitHub email as this helps your contributions to reflect on your profile.
    



# 3. Stages in Version Controlling Using Git (Modify, Stage, & Commit)
<p>a. MODIFY - This involve changing and saving your codes.</P>
<p>b. STAGE - Before a modified code can be tracked or commited, it has to be stagged. Use the following commands to stage your codes:</P>
  <p><b>git add fileNmae</b>  or <b>git add . </b>  (to stage more than one file).</P>
 <p> <b>git status</b>  (to check if your files has been staged).</p>
<p>c. COMMIT - This is done after stagging your codes. At this point, you seem satisfied with what you have written and you want it to be trackable. Use the following commands for commiting your codes: 
  <p><b>git commit -m "commit name" </b> then press enter. </p>NB: Commit name helps you to remember what that code is all about. E.g "added index.html"
<p>  <b>git log</b> (to view your commit history)</p>
 <p> <b>git log --oneline</b> (to view your commit history in one line).</P>
  
  
  
# 4.  Git Undoings (Checkout, Revert & Reset)
  CHECKOUT - helps to navigate from one commit to another in a particular code branch. Use the following commands to checkout or navigate your commits or branch
 
    git checkout commitID (NB: commitID can be obtained when you check your commit history)
   <P> <b>git checkout master</b> (to navigate to the master branch).</P>
  <p> <b> git checkout branchName</b> (to naviage to another branch other than the master branch).</p>
    
<p> <b>  REVERT</b> - helps to create another commit after modifying a particular commit of a particular branch. For example, you have a commit called "hello world", containing "Hello world" as the content. If you want to change the content to "Hello Nigeria", you need to make another commit by reverting the "hello world" commit. This preserves the "hello world" commit and also produce a new commit e.g "Hello Nigeria".  Use the steps below for reverting your commit:</p>
    <p>1. Stage your code by entering <b>git add .</b> </P>
  <p>  2. Revert your commit by entering <b>git revert newCommitName</b> then press enter</P>
 
<p> <b> RESET</b> - When you reset a commit, all the commit history before it will be deleted. Lets assume we have the following commits: <p> a->b->c->d->e->f</p> When we reset our commit history to e, commits a,b,c and d will be deleted. Use the command below to reset to a commit:
<p>   <b> git reset desiredCommitID --hard</b></p>
    
 
 

  
 # 5.  Branching
  Branching helps to introduce new fetures to your app without affecting the master branch. NB: The master branch is the stable version of your app and its the repository or folder that was created when git is initiated.
  <P>To create a new branch, use the following commands:
      <P> <b>git branch branchName</b></p>
   NB: You have to checkout your new branch before you can stage or make commits in it. Use the following commands to checkout or navigate to a branch: 
  <p><b>git checkout branchName</b></p>
   <b>git checkout -b branchName</b> (to create and checkout a new branch simultaneously).</p>
   <p> You can delete a branch by using <b> git branch -D branchName </b>.</p>
  <p> NB: You must be in the master branch to delete any branch </p>
   
   
   
# 6. Merging Branches
  Branches are usually merged when the developers are satisfied with the commits of the new branch and no conflicts exist.
  <p> Use <b> git merge branchToBeMerged </b> </p>
  
  <p> NB: You must be in the master branch to merge any branch with it </p>
  
# 7. Introduction to GitHub
  GitHub is the remote or online version of Git. It also allows collaborating and sharing repositories with other developers.
  
  
# 8. Pushing (local to remote)
    Pushing involves transferring your Git repository to the GitHub repository. 
    This is useful when you already have a local Git repository and you want to sync it with your online GitHub account.
    Follow the steps below to push to your remote repository.
    
*  Create a new repositroy on GitHub and give it same name as your local repository.
*  Decide whether its public or private.
*  Copy the url of the new remote repository.
*  Go to the command line on your local repository and enter: <b>git push url master</b>
*  NB: Always specify the branch you are pushing to.



# 9. GitHub Alias
  * Alias are used for naming or tagging your remote repository url. Instead of copying and pasting a long url, the alias shortens it.
  * Enter <b> git remote add origin url</b>
  * NB: the origin above is the alias name and can be named differently.
  * When pushing with alias, use <b> git push origin master </b>
  
  
  # 10. Pulling or Cloning ( remote to local)
  *  Pulling/cloning is used when you want to download a repository that does not exist on your local machine. 
  * On the right-hand side of your remote repository, click code button and copy the url under https.
  * Go to your local terminal and set the path to the directory you want your repository to be.
  * Enter <b> git clone url </b>
  * NB: When pushing codes back to your remote repository, you do not need to create another alias. Github cloning automatically gives your repository an alias called "origin".
  
  
  # 11. Collaborating on GitHub (privately and publicly)
  * When working privately with your team, follow these steps to make your contributions:
    * For already cloned repository, enter <b> git pull origin master</b> in the local terminal to sync your local repository with your remote repository.
    * Create a new branch(to avoid messing up the master branch in case of errors).
    * Add your contributions in the new branch
    * Stage the new changes
    * Commit the changes
    * Push the branch to the remote.
    * Use <b> git push origin branchName"</b> to push the branch.
    * Go to GitHub and make pull request for others to approve your contributions.
    * Once approved, your project manager will merge this branch with the master branch.
    
  * When working on public projects, forking is used to collaborate.
  * Use the steps below to to contribute to an open source project:
    * Fork your desired open project
    * Clone the repository on your local machine
    * Make a new branch and make your contributions.
    * Stage and commit your contributions.
    * Push your contributions to the remote repository
    * Click pull request for approval
    * Once the project manager is satisfied with your contribution, it is merged with the master branch.


NB: when you lost your local repo and your pushing the new changes to the remote repo, use these commands:
git push -f <repo name> master  (for first push)
  or git push <repo name> master (if you have pushed before)
    

  
    
    

  
  





