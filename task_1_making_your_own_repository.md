# Create your first repository and add it to GitHub

1. Set up your local repository
  * On the command line, go to a folder you'd like to add as a repository to GitHub or create an empty folder
  * type `git init`  
  * What happened? (check `ls -la`)

2. Add something  
Once you've created a repository, you can start editing it! An easy first step is that you create a new text file and add it to the repository. 
   * create a new .txt file in the folder (you can use `touch <filename>` on the command line or just create a file on any text manager you normally used)
   * `git status`
   * stage the changes with `git add .`
   * `git status`

3. Commit your changes  
  * `git commit -m "<your commit message>"`
  Traditionally the commit message for the commit is "Initial commit", but feel free to use whatever you want. 
  Tip: if you forget to add -m <commit message>, you will be thrown into a terminal text editor to write the commit message. For some mysterious reason the default text editor tends to be vi, which is not very intuitive. To escape, press 
`:q <Return>` (note the colon, which toggles between typing and commands in vi). You can also set your default text editor for git with `git config --global core.editor <yourpreferrededitor>`
(see options and other useful settings at https://swcarpentry.github.io/git-novice/02-setup/index.html)


4. Repeat steps 2 & 3 a few times 
  You can add files and modify files as you wish. If you're working with code files or plain text files, you can use `git diff` to see the difference between workin directory and staged files. Even though you're just playing around, you can also think about commit messages - they should be informative and unique (so, not just "added a file").

5. Create a new project on GitHub
So far your changes have all happened on your own computer. This next bit enables you to save any changes you committed to GitHub, which will keep them backed up & you can share your progress with collaborators or lab members
  * go to github.com
  * create a new repository by clicking the "new repository" button on the top right hand corner  

6. Add your newly created project as a remote to your local repository
  * `git remote add origin YOURORIGINADDRESS` 
  You can find your origin address on your new repository, under the button 'clone or download'. If you have ssh keys set up, use SSH, if not, use HTTP.
  * Check your remote with `git remote -v`
  * _push_ your version to the origin with `git push origin master`
  * go check the repository online to see your changes
  * check commit history with `git log --oneline`

7. Create a .gitignore (optional)
  If you're working on an existing project, there are likely some files that you know you don't want to share. This may include data files (do not put data files on repositories!!), files created by your filesystem (.DS_Store on macs) or any files you're just using for testing. To stop git showing them as something you'd like to add, you can create a file called .gitignore
  * `touch .gitignore`
  * Add files or patterns you want git to ignore, each separated by newline
  * For an example of generic .gitignore, see https://gist.github.com/octocat/9257657

8. Advanced: Try to undo something you've done 
One of the best reasons to use version control is that you can undo pretty much anything that you've done at any point in the history of the code. There are a few different ways to do this depending on how far you got with that change. A nice explanation can be found e.g. here https://github.blog/2015-06-08-how-to-undo-almost-anything-with-git/ . This is a nice diagram for reference https://raw.githubusercontent.com/emmajane/gitforteams/master/resources/workflow-undoing-changes.png
