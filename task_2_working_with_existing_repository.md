# Write a poem in your group

This exercise is a short introduction to how you would typically use version control in a team. You might run into some technical difficulties, but more likely it'll go just as smoothly as the previous task. Moreover, I'm available to answer questions and help you troubleshoot during the Q&A. 

1. Create an online repository and share collaborator privileges
 In order to complete this exercise, have one in your group create a new repository and add others as 'collaborators' to a repository on github using these instructions https://help.github.com/en/github/setting-up-and-managing-your-github-user-account/inviting-collaborators-to-a-personal-repository.
 Then, all of the team members should do the following
   * using your command line interface, navigate to the parent folder where you want to add the repository
   * _clone_ an existing repository with `git clone`  
(use the https address if you do not already have ssh keys set up)
   * take a look in the repository
   * run `git status` (inside the folder)
   
   _NB: Do not run `git init` before you `git clone` - the cloning does init too!_

2. (Everyone) Create a .txt file 
  In that file, write a few lines that could be the beginning of a poem written by a kindergartener. E.g.
  "There was a little mouse / 
  Who had a little house"

3. _Stage_ and _commit_

4. Share your change with others
   * check to see that you've got the remote repository set with `git remote -v`
   * make sure your local version is the latest version by _pulling_ the latest version from the remote `git pull origin master`  
   * Push your repository to _origin master_

5. Try editing something 
By this point, hopefully someone else has also pushed their changes to your remote. 
   * get the latest changes with pull
   * edit a text file someone else has created by adding two more lines to somwhere in their poem
   * `git status`
   * You can also try `git diff` to see the changes
   * _stage_
   * `git status`
   * _commit_, _pull_, and _push_ as above  
   NB: If someone has changed the exact lines of text you have, you might get a conflict when you pull. This means that git doesn't know which changes are the ones to keep - the ones on the remote or the ones you just made. Ask for help or check e.g. https://swcarpentry.github.io/git-novice/09-conflict/

5. Advanced: try creating a branch and editing that  
Typically you would not go directly editing someone's code unless you're actively collaborating on it. Even then, it is a great idea to create a branch, where you can work and break things without impacting the main code. Then, once your addition is ready, you can _merge_ it (i.e. you yourself add it to the main development line) or submit a _pull request_ (i.e. you ask the owner of the code or someone else to take a look at your code and add it to the main development code).  
If you want to try branching, this https://coderefinery.github.io/git-intro/06-branches/ seems like a very good tutorial to follow. Instead of ingredients.txt, just do some random edits to any text file in the repository.  
NB: if you work on a branch, you would `git push origin [branchname]` since you want to commit the changes made to your branch, not changes made to the master (main development line). You can also try branching in an online sandbox here https://learngitbranching.js.org/ .



