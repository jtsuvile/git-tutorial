
1. Get a repository  
This is what you would do if you wanted to use and modify a set of code ('repository') that someone else has created. For example, an analysis code your colleague has already written.
   * using your command line interface, navigate to the parent folder where you want to add the repository
   * _clone_ an existing repository with `git clone`  
(use the https address if you do not already have ssh keys set up)
   * take a look in the repository
   * run `git status` (inside the folder)

2. Add something  
Once you've cloned the repository, you can start editing it! An easy first step is that you create a new text file and add it to the repository. 
   * create a new file in the folder, name it with your name
   * `git status`
   * stage the changes with `git add .`
   * `git status`
   * _commit_ your change to the repository `git commit -m "added file X"`

3. Share your change with others
So far your changes have all happened on your own computer. This next bit enables you to save any changes you committed to GitHub, which will keep them backed up & you can share your progress with collaborators or lab members
   * check to see that you've got the remote repository set with `git remote -v`
   * make sure your local version is the latest version by _pulling_ the latest version from the remote `git pull origin master`  
   * _push_ your version to the origin with `git push origin master`
   * go check the repository online to see your changes
   * check commit history with `git log --oneline`

4. Try editing something 
   * edit a text file someone else has created 
   * `git status`
   * You can also try `git diff` to see the changes
   * _stage_
   * `git status`
   * _commit_, _pull_, and _push_ as above  
   NB: If someone has changed the exact lines of text you have, you might get a conflict (i.e. git doesn't know if you want to keep the remote version or the local version). Ask for help or check e.g. https://swcarpentry.github.io/git-novice/09-conflict/

5. Advanced: try creating a branch and editing that  
Typically you would not go directly editing someone's code unless you're actively collaborating on it. Even then, it is a great idea to create a branch, where you can work and break things without impacting the main code. Then, once your addition is ready, you can _merge_ it (i.e. you yourself add it to the main development line) or submit a _pull request_ (i.e. you ask the owner of the code or someone else to take a look at your code and add it to the main development code).

If you want to try branching, this https://coderefinery.github.io/git-intro/09-branches/ seems like a very good tutorial to follow. Instead of ingredients.txt, just do some random edits to any text file in the repository.



