# Laboratory of Computational Physics (mod. A)

This is the official repository of the course, and contains the Jupyter Notebooks guiding students through the world of data analysis with python.

This repo should be forked by each individual student. 

Git instructions are provided in the dedicated README files in the repo.

## IPython notebooks instructions and tips

Notebooks are extremely powerful tools, you may find useful to discover some of their functionalities on this tutorial [page](https://nbviewer.jupyter.org/github/ipython/ipython/blob/3.x/examples/Notebook/Index.ipynb) or by checking these tips [list](https://www.dataquest.io/blog/jupyter-notebook-tips-tricks-shortcuts/)

## Git instructions

To begin with, you need to have a GitHub account. If you don't already have one, go to [github](github.com) and sign up. Follow instructions on the screen. Tip: use a reasonable username that resembles your actual name.  

Once you have your github account, fork this repository clicking on the top-right button *Fork*.

Generate your Token on GitHub following this [guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token). Copy the token to a safe place. Remember you can see it only the first time, otherwise if you lose it you have to create another one.



### Standard development cycle

   * Before starting with the development you could check whether the upstream repository has been updated with respect to your forked version (that's likely to be the case prior to every lab class). If it had, then merge the changes into your main:

   `git checkout main`
   
   `git fetch upstream`

   `git merge upstream/main`
   
   * And then in your development branch, if any:
   
   `git checkout <BranchName>`

   * The idea is that your main always reflects `upstream/main`, i.e. it keeps a local copy of the reference code as a starting point for your developments (i.e. solving the assigned problems). Note that in order to update your repository on GitHub, you need to push the local version to your remote repository.

   * Before starting to edit on the machine that you are using, type the follow command in order to update the directory with the last changes:
  
   `git pull`
   
   * You may also need to get the updates from the main, i.e. need to merge the main:

   `git merge main`

   * If you create a new file <NewFile> you need to tell git to track
      it
	  
   `git add <NewFile`
   
   * Commits the (tracked) changes you made to the file(s) and commit
     them local repository on github
	 
   `git commit -m "some comment"`
	 
   (what follows after -m is a comment to keep track of the reason of the commit)

   * Now propagate (push) your local changes to your remote repository
     on github (`origin`)
	 
   `git push origin <BranchName>`

   * If on the other hand you want to keep the local modifications somehow, you'd use stash to hide them away before pulling, then reapply them afterwards:

	`git stash`
	
	`git pull`
	
	`git stash pop`


