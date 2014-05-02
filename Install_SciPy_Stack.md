#SciPy Installation Guide
##Objective
We will be using Anaconda/Miniconda 3 to get SciPy stacks up to date and running on your Ubuntu OS.

#Intuition about SciPy || Anaconda || Miniconda 3
SciPy: http://www.scipy.org/about.html
Anaconda: https://store.continuum.io/cshop/anaconda/
Miniconda 3: 


##Step 1
Go to http://continuum.io/downloads and download your Linux machine's installer. It will be one of the two options below.

-Linux 32-bit / 411M / md5: c8f72746dd5dc68f014d5fccd1f060e8
-Linux 64-bit / 483M / md5: 863ee49f52bda17810ab1b94a52f8c95 

##Step 2
Once the Anaconda installer is download, open a terminal and navigate to installer's location and run:

-$ bash Anaconda-1.x.x-Linux-x86[_64].sh

Replace the 1.x.x in the command above with the version number from the downloaded installer file.
After accepting the license terms, you will be asked to specify the install location (which defaults to ~/anaconda).

##Step 3
Add Anaconda to your PATH environment variable, if not already done so with the command below:

export PATH=~/anaconda/bin:$PATH

##Step 4
The following command would be used to create an Anaconda Python 3 environment named py3k:

$ conda create -n py3k python=3 anaconda

##Step 5
After adding the binary directory of the newly created environment to the PATH environment variable, which may be done using:

$ source activate py3k

##Step 6
To update Anaconda use:

$ conda update conda
$ conda update anaconda

Even if your Anaconda is at it's most recent update after installation, these commands will help you practice updating your software.

##Step 7
The following command will download and install the SciPy stack:

sudo apt-get install python-numpy python-scipy python-matplotlib ipython ipython-notebook python-pandas python-sympy python-nose

After the above command is ran, the terminal will tell you what packages need to be installed and which ones are already up to date.
The terminal will prompt you to download these files and ask if you want to continue.

After this operation, XXX MB of additional disk space will be used.
Do you want to continue [Y/n]? Y

##Step 8
Do not exit the terminal window while downloading.

References:
http://www.scipy.org/index.html
http://www.scipy.org/install.html#scientific-python-distributions
http://continuum.io/blog/anaconda-python-3


