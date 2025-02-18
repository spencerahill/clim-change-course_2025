# Using the course JupyterHub

**LINK TO THE JUPYTERHUB: https://ccny25s-1.ees220002.projects.jetstream-cloud.org**

## Overview

We will use the Python programming language running within Jupyter notebooks to perform quantitative analyses of some climate datasets, run simple models, and other tasks.  If you aren't familiar with these, or even programming at all, that's ok, there is no programming prerequisite.  Jupyter notebooks are a way to work with code that makes it easy enough for novices to follow along too.

Any code ultimately has to have some computer to run on.  In principle, that could be your own computer, provided you downloaded and properly installed python, jupyter, and all the other requirements (which isn't as hard as it sounds, at least if you're not on Windows, but I digress).  

Rather than having each of you do all that installation and setup and forcing you to bring your laptop to every class, we will run these notebooks on a cloud-based server, called a JupyterHub, setup specifically for this class.

## Getting access to the JupyterHub 

### Step 1: Create a free Github account if you don't already have one

To make sure only students in the course can access the JupyterHub, you'll have to login using a Github account.  If you don't alreaady have one, they are free and take only a few minutes to setup: go [here](https://github.com/signup).

### Step 2: Submit your Github profile name via Brightspace

There is an assignment within the course Brightspace where you submit your Github profile name.  Once you've done that, the professor will be able to add you as one of the approved users of the JupyterHub.

### Step 3: Login to the JupyterHub.

The link to the course JupyterHub is at the top of this page and repeated [here](https://ccny25s-1.ees220002.projects.jetstream-cloud.org).  Once you've been added as an approved user, go there and login using your Github profile.  

You'll get a warning message about "Authorize JupyterHub CCNY Spring 2025 by Ana Espinoza."  Ana Espinoza is the sysadmin who is running the JupyterHub for us (thanks Ana!).  So go ahead and accept that.  Then, you should be able to login and end up at the Jupyterlab.

### Step 4: Check that it works

:::{note}
If you're already familiar with how to use Jupyterlab, then simply do things you normally would and see if they work: create a new notebook, run some cells, etc.  As long as that all works, it means the Jupyterhub server is up and running correctly.  If you *don't* know how to do all that, follow the instructions below.
:::

Once you successfully login, your browser will show a main window called the "Launcher", and to the left of that a narrower column that looks like a file explorer you're familiar with on your computer.   In the Launcher window, the the heading at the top will say "Notebook", and just below it will be two squares with blue and yellow symbols inside.  Click the one on the **right** that says `Python [conda env:ccny25s]`.

This will create a new, empty **Jupyter Notebook** and open it in that window, replacing the Launcher window.  Click inside the long skinny rectangle near the top; this is an empty **cell**.  When you click inside it, you'll be able to type things into it.  Type the following, and don't forget the quotation marks: `print("hello world")`.  Then, in the bar at the top of the notebook window, press the right-pointing triangle that looks like a "play" button on a remote.  Just below the cell, there should 

:::{note}
If instead you get some kind of error message, that still means the server is working!  Most likely, you forgot one or both quotation marks or parentheses, or accidentally misspelled `print`.  Of course, you're welcome to try to **debug** the problem by changing the text and re-running the cell, repeating that as needed until it works.  But for the purposes of verifying that the Jupyterhub server is working properly for you, mission accomplished!
:::
<!-- In that left column, there is a folder named "`share`".  Double click it.  Inside will be a file named `our-first-jupyter-notebook.ipynb`.  Double click that file.  It will open up in the bigger window to the right, replacing what was the Launcher.  
 -->
## Troubleshooting

### "The connection has timed out"
On occasion, the JupyterHub server goes down, for reasons completely out of our control.  So if you enter the URL correctly and your browser gives you an error message along the lines of "the connection has timed out", please give it ~10 minutes and then try again.

If you still can't access the JupyterHub after 1 hour of trying, please email the professor.

## Credits

This JupyterHub was setup and is being administered for us as a free service from Unidata.  The actual physical computer it lives on is at the University of Indiana.  Thank you Unidata, and go Hoosiers!