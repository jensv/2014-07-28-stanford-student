#Git Exercises

##Pre-Lesson

Create a new directory, called `git-project`, NOT inside the directory we used yesterday (see diagram on board).  
Then copy the directory `project_files` from the cloned git directory to this one.  You can do this using your mouse, or, 
if you're feeling brave, using shell commands.  A sample series of commands might be: 

~~~
$mkdir git-project

$cp -r (link) git-project/
~~

Look around at the files you've just moved.  If you have time, please make an account on GitHub - we'll need it later in the lesson.  

## Modifying files and committing changes

In `stats-script.sh`, redirect the output of goostats to a file called `output.txt`.*  Then add and commit your changes.  

(To redirect, just add `>> output.txt` to the middle line of the script.)  

##Review

Think about all the commands and processes we've talked about so far.  Try to diagram/flowchart a project workflow 
that includes all these ideas and annotate with the appropriate git command.  

##Remote practice

Edit the README so that it's more descriptive, then commit and push changes to your repository.  

##Remotes and automation

What if you wanted to work on material in someone else’s directory/repository that's hosted online?  Which shell/git commands would you need to "download" the other person's repository onto your computer?  

* Hint 1: This should take around 5 commands

* Hint 2: There are 2 shell and 3 git commands.  

* Hint 3: The sequence of events is a) create a directory to store the files, b) move into that directory, c) initialize that directory as a repository, d) link the other person's remote repository and your local repository, e) move the files from that remote to your local.  

##Collaboration

###1
Pair up with someone next to you.  Go out of `project_files` into `git-project`.  (`cd ..`)  Then clone your neighbor's repository to your computer using:

~~~
git clone (https://github.com/ ... ) (choose a name for the cloned directory on your computer)
~~~

Go into the cloned repository (use `cd`) and add a file named "paper.txt", with a title and both of you listed as authors.  Stage + commit the file.  Now try pushing to their repository (which should be named `origin`).  What happens?  

###2
After your partner has added you to their repository on github, try pushing again.  Look at what your partner has pushed to your online repository.  How do you get their additions to your files into your local copy?  

###3
Make changes in your copy of `paper.txt`.  Push them to your repository.  

###4
Switch to your local copy of your partner's repostitory and edit their paper (make lots of changes - delete things, add a paragraph, whatever).  **Don't pull from your partner's repository beforehand.** Now try to push your changes to their online repository.  What happens?  

###5
Pull down their changes.  What happens now?  

###6
Via `git push` and `git pull`, write a biography for yourself in both your copy of the paper and your partner's copy, so at the end, each of you has both biographies in their copy of `paper.txt`.   

## Review

Make a diagram depicting your remote repository and its two local copies (one on your computer, one on your neighbor's).  Add notes, labels and/or the appropriate git commands as desired.  

##Shell review

Try to modify the `stats-script` file so that instead of placing results in a single output file, each result from an input file gets sent to a file named `stats-$datafile`.  

## Review

There are several features of version control we've tried out today.  For each topic below, write down the associated commands in git, and one example from your own work where you could use this (even if it's unlikely you'll be able to implement it).  

* Saving "versions" of your work with annotations: 
* Storing a copy of your work online: 
* Sharing files with others via an online repository: 
* Restoring previous versions of files: 
* Maintaining multiple versions of a project: 
