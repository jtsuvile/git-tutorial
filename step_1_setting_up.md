# Steps to get started

1. Make sure you have a functional git installation and a command line system to go with it

You can check to see if you already have git installed by writing `git version` on your console. If you don't already have git, you need to install it. If you have Ubuntu for Windows or you're working on an unix-based system, this can be as easy as 
`sudo apt-get install git`. For Windows, see https://git-scm.com/

2. Configure your git

Set your name and email on your local machine by running the commands below (except with your own information, naturally)
```
git config --global user.name "John Doe" 
git config --global user.email johndoe@example.com 
``` 

3. Set up a key pair to access git

Create a key pair on your computer, [see instructions here](https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) OR you can install [GitHub Desktop](https://desktop.github.com/). (Most tutorials assume that you use command line and I will point to directions that use command line, but the underlaying logic is the same)

4. Make sure your connection works by running `ssh -T git@github.com`
