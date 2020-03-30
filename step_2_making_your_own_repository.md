1. Set up your local repository
  * On the command line, go to a folder you'd like to add as a repository to GitHub or create an empty folder
  * type `git init`  
  * What happened? (check `ls -la`)
  * If you started with an empty folder, make a file

2. Stage the files you want to include in the repository

3. Create a .gitignore (optional)
  If you're working on an existing project, there are likely some files that you know you don't want to share. This may include data files (do not put data files on repositories!!), files created by your filesystem (.DS_Store on macs) or any files you're just using for testing. To stop git showing them as something you'd like to add, you can create a file called .gitignore
  * `touch .gitignore`
  * Add files or patterns you want git to ignore, each separated by newline
  * For an example of generic .gitignore, see https://gist.github.com/octocat/9257657

4. Commit your changes  
  Typically the commit message for the commit is "Initial commit", but feel free to use whatever you want

5. Create a new project on GitHub
  * go to github.com
  * create a new repository by clicking the "new repository" button on the top right hand corner  
  If this repository is something you don't want to share, you can create it under your own user space. If it is something the team would benefit from, you can create it under https://github.com/tndrg/

6. Add your newly created project as a remote to your local repository
  * `git remote add origin YOURORIGINADDRESS` 
  You can find your origin address on your new repository, under the button 'clone or download'. If you have ssh keys set up, use SSH, if not, use HTTP.
  * Check your remote with `git remote -v`
  * Push your repository to _origin master_

7. Advanced: Try to undo something you've done 
One of the best reasons to use version control is that you can undo pretty much anything that you've done at any point in the history of the code. There are a few different ways to do this depending on how far you got with that change. A nice explanation can be found e.g. here https://github.blog/2015-06-08-how-to-undo-almost-anything-with-git/ . This is a nice diagram for reference https://raw.githubusercontent.com/emmajane/gitforteams/master/resources/workflow-undoing-changes.png
