
1. Get a repository
   * _clone_ an existing repository with `git clone`  
(use the https address if you do not already have ssh keys set up)
   * take a look in the repository
   * run git status

2. Add something
   * create a new file in the folder, name it with your name
   * `git status`
   * stage the changes with `git add .`
   * `git status`
   * _commit_ your change to the repository `git commit -m "added file X"`

3. Share your change with others
   * make sure your local version is the latest version by _pulling_ the latest version from the remote `git pull origin master`  
   NB: If someone has changed the exact lines of text you have, you might get a conflict (i.e. git doesn't know if you want to keep the remote version or the local version). 
   * _push_ your version to the origin with `git push origin master`
   * go check the repository online to see your changes
   * check commit history with `git log --oneline`

   4. Try editing something 
   * edit a file someone else has created 
   * `git status`
   * _stage_
   * `git status`
   * _commit_ and _push_ as above