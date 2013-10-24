projectX
========

This isnt exactly a project description, rather a quick Getting Started to Git.

Firstly, to download the latest copy to your computer (ONLY if you haven't downloaded a copy yet)

	git clone https://github.com/fosscell/projectX.git

Running that command creates a new folder projectx in your home dir. This is your local copy of the project.
Now cd into that directory using terminal and execute the following commands :

  a) If you're using an SSL or some other shared computer. Repeat each time before you begin using that computer. This is local to the project only and wont affect other projects.
  
    git config user.name "My Name Here"
    git config user.email "My eMail ID"
    
  b) If you're using your own computer, you only need to run this just the one time and it'll persist accross all projects.
    
    git config --global user.name "My Name Here"
    git config --global user.email "My eMail ID"
    
Now, you're configured to use the code. Lets say someone made some changes to the remote repository (GitHub in this case) and you want to have those same changes in your local copy, do

	git pull
  
Note that git might throw up an error or two if you have some uncommited changes. The error itself will probably provide you the method to fix it so always read errors from git commands.
Now, you have the latest code. Always do a git pull before pushing your commits to prevent issues due to mismatched history. (Similarly do a git pull to get the latest code before starting work in case someone made changes in the meantime) 

You can now make edits to the local copy. Lets say you made a few changes to add some feature X. We create commits for certain checkpoints such as the changes to implement a specific feature. Now, we will create a new commit to show the changes made for this feature. Firstly, type the following command to see exactly what changes you made

	git status

The changes you make will all be shown here. To add a particular file to the commit, type
	
	git add filename

Once you've added all the files you want to add, you can create the commit by typing 

	git commit -m "Added Feature X"

Make sure that the message you add to the commit is meaningful and clearly mentions what the commit is meant to do. After creating a commit, you can either continue making changes and add more commits or push the changes to the remote repository. Again, dont forget to do a git pull first to get any code changes others may have made before pushing. Once your local repo is ready, type

	git push

This will upload your commits to the repo and others can view your work. This covers the basics of things. Most other doubts can easily be clarified via tutorials or through google searches for the same.

Happy Gitting!
