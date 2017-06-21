# github_workshop

##Please do the following before we start

**** Note that this workshop will focus on using GitHub with the terminal, which Mac and Linux OS already have. Otherwise, I recommend installing a terminal emulator, and making sure you have git installed. ****
***** Set up yourself with a GitHub account if you haven't already [here](https://github.com/)****
***** Make sure you have a text editor installed that you are comfortable with

### What is GitHub and how does GitHub work

####History
* GitHub is a version control system for tracking changes in computer files and coordinating work on those files among multiple people
* Was created in 2005 for development of the Linux kernel, but unlike the linux kernel, it is FREE

####How it works

[![GitHub Visualization](https://camo.githubusercontent.com/d4de2fdb747fec0d3dc67b1640f37c12f3786f5b/687474703a2f2f6a6c6f72642e75732f6769742d69742f6173736574732f696d67732f72656d6f7465732e706e67)
*****
*
*
*
*

### Getting Started

1. Open up your terminal and type cd ~/Desktop to navigate to your desktop (cd is change directory)
2. Open up a browser, and go to the repository for this workshop [here](https://github.com/ByronBecker/github_workshop)
3. In the upper right hand corner, click Fork to fork the repository (this makes a copy of the repository on your remote GitHub Server for your account
4. Now click on the green clone or download button, and copy the link that appears  
5. Back in the terminal, type git clone paste_of_link_you_just_copied          
This should clone a copy of the repository as a folder titled github_workshop to your Desktop
6. Now change directory into github_workshop. Experiment with the following commands, what do you think each does?
    a) git status
    b) git pull origin master
    c) git push origin master
    d) git remote -v

*7. ****Now open up hellopython.py in your favorite text editor, and add the following line somewhere:    print("I just changed this file")
    - repeat step 6 (Note: you WILL get errors for each, why do you think so?)

After changing any files in the repository, you have to do the following steps.
    recommended (optional) first step: git status to check what has changed since the last commit
    i) git add (name of file that was changed)
    ii) git commit -m "insert descriptive message here of what you changed/added"
    iii) git push origin master   (this is the default name of your fork)
    

### Resolving Merge Conflicts!

* A merge conflict is when the git system doesn't know what to do with two different versions of the same file where certain parts have been overwritten, how does the computer decide who is right? => Merge conflict
* This can be one of the most frustrating parts of GitHub!
* We are going to now create a merge conflict and resolve it!

1. Go to the hellopython.py file in the browser and edit it as I do  !!! Never edit files directly in the browser other than for this example !!!
2. Now go to your hellopython.py file on your computer, and add the line: print("Changing the file")
3. Now go through steps 7i - 7iii of Getting started, it should return the following
        ! [rejected]        master -> master (fetch first)
        error: failed to push some refs to 'git@github.com:ByronBecker/github_workshop.git'
        hint: Updates were rejected because the remote contains work that you do
        hint: not have locally. This is usually caused by another repository pushing
        hint: to the same ref. You may want to first integrate the remote changes
        hint: (e.g., 'git pull ...') before pushing again.
        hint: See the 'Note about fast-forwards' in 'git push --help' for details.

    - From the message, what do you think we should try next?

5. If you said "git pull origin master", you were right, try that...

    - we now have our Merge conflict => GitHub wants YOU to be the fixer and decide which lines to keep, and which to throw out

6. Open up hellopython.py in your text editor, you should see something like this

    <<<<<<< HEAD
  print("Hello World")
  print("Changing the file")
  =======
  print("I created chaos")
  print("Helsinki World")
  >>>>>>> 6480f217bb9413dd62753f3efb50b60e819c5f9f

  - the <<<< HEAD to ==== represents your copy of what you were just about to push, and the ===== to >>>>>> represents what was stored in the last commit (number of commit) on your remote repository.  

7. fix your code so it contains what you want, make sure to delete the <<<HEAD, ===, and >>>commit number, and then save the file

8. Type git status. Now what do you think you need to do now to commit the change and push it to your remote?


### Clearing Unwanted Changes

What happens if just commited some changes and pushed them, and then worked for about 30 minutes on something you really don't like anymore. You want to revert to the last commited copy of your files

git reset --hard   => this resets any and all changes in the working tree since the last commit



### GitHub Etiquette





### Forking vs Branching
