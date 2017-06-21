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
    b) git pull
    c) git push origin master
    d) git remote -v

*7. ****Now open up hellopython.py in your favorite text editor, and add the following line somewhere:    print("I just changed this file")
    - repeat step 6 (Note: you WILL get errors for each, why do you think so?)

After changing any files in the repository, you have to do the following steps.
    i) git add (name of file that was changed)
    ii) git commit -m "insert descriptive message here of what you changed/added"
    iii) git push origin master   (this is the default name of your fork)
    

### Clearing Unwanted Changes



### Resolving Merge Conflicts!







### GitHub Etiquette



### Forking vs Branching
