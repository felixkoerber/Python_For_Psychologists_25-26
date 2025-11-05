# Setup for the course

There are a few things you need to get working on your computer in order to follow this course. However, don't worry as it's all gonna be [open source](), won't require a lot of storage and will be explained in detail.

In general getting `Python` & friends to work reliably on your machine is going to be very beneficial. This holds true for the course but also beyond. The following tools focusing on open and reproducible (neuro-/data-) science) will therefore not only be necessary for this course, but may allow you to build an "everyday" research workflow around them, for example when writing your Master's thesis. This even applies if you won't continue with `python` (I certainly hope you do) and instead work with `R` (of course also cool), `matlab` (weeeeeeeell...) or what have you. 

You'll find the (hopefully) comprehensive set of install instructions below. We first focus on just two core pieces of software, and may at later points potentially add more.   

Don't worry, you got this!

![logo](https://media1.tenor.com/images/f72cb542d6b3e3c3421889e0a3d9628d/tenor.gif?itemid=4533805)\
<sub><sup><sub><sup>https://media1.tenor.com/images/f72cb542d6b3e3c3421889e0a3d9628d/tenor.gif?itemid=4533805</sup></sub></sup></sub>


## General things

There are a few computing requirements for the course that are absolutely necessary (beyond the few software packages you should install, described below):

1. You must have administrator access to your computer (i.e., you must be able to install things yourself without requesting IT approval).
2. You should have at least 20 GB of free disk space on your computer (but we would recommend more, to be safe).
3. If you are using Windows you must be using Windows 10/11; Windows 7 and 8 will not be sufficient for this course.

If you foresee any of these being a problem please reach out to one of the instructors and enquire what steps you can take to ensure your setup is ready for the course.

## Required software

To get the most out of the course, we ask that you to install the following software (software/things in () are not entirely necessary but definitely great to have):

- `Python 3` via [`Miniconda`](https://docs.conda.io/en/latest/miniconda.html)
- An remote-capable text editor, also called IDE or integrative development environment : [`PyCharm`](https://www.jetbrains.com/pycharm/)
- A `modern web-browser`. Unfortunately, macOS users may want to have a different browser besides 'Safari', like 'Firefox' or 'Chrome'.

Miniconda is a frequently used system in scientific computing that contains python, but also is an efficient way of keeping your software packages up to date and of managing the environment in which you conduct scientific computing (like data analysis). PyCharm is a powerful user interface, which we will use to run interactive python notebooks but which also provides us with a terminal window through which we can do other things like installing packages or managing our computing environment. The web browser is not strictly necessary, but for our first steps using interactive jupyter notebooks, we will use the browser. 

If you already have the above software tools/packages installed (what are you even doing here?), or are confident you’ll be able to install them by the time the course starts, or a have enough programming experience that you have alternative installations with similar functionality, you can use these. 

There are a number of further software that may become relevant in the next weeks, but do not have to be installed right now. These influde:

- (Most likely [`Discord`](https://discord.com/) for communication purposes)
- (A command-line shell: [`Bash`](https://www.gnu.org/software/bash/), already included in macOS and LINUX, and under windows probably best to use 'gitbash', which comes with the 'git' package, see next bullet point.)
- (A version control system: [`Git`](https://git-scm.com/))
- (A [`GitHub`](https://github.com/) account)


The rest of this page provides more detail on installation procedures for each of the above elements, with separate instructions for each of the three major operating systems (`Windows`, `Mac OS`, and `Linux`).


### Some quick general notes on instructions

- There is no difference between `Enter` and `Return` in these instructions, so just press whatever the equivalent on your keyboard is whenever one is stated
- If you already have some of these things installed on your computer that should (theoretically) be okay.
- Having multiple different `Python` installations on your computer can lead to frustrating issues that are very difficult to debug. Thus, if you have already installed `Python` via some other application (not `Miniconda`/`Anaconda`), it's strongly encouraged to uninstall it before following the instructions below. Alternatively, you should (be able to) assure that the basic needed functionality works in your setup. At the moment, this primarily involves running python interactively in jupyter notebooks.


### OS-specific installation instructions

Select the tab that corresponds to your operating system and follow the instructions therein.

````{tab-set}
```{tab-item} Windows

**Python**

1. Go to the Anaconda website and follow the guidelines for the installation instrcutions: https://www.anaconda.com/docs/getting-started/miniconda/install#windows-installation . Please read through the following points before installing!
2. This will take you also to the download page on their website. Note: Please ignore the box on the top right that says "Download now. Get access in 30 seconds.". Rather, go to the very bottom of the download page and click the button saying 'Download Miniconda Installer'. Here, select on the right side the 'Miniconda Installer', download it and run it. 
3. The installation guideline webpage also notifies you that it makes sense to select the 'Just Me ...' option, which means that miniconda is installed into your personal user account, and that it makes sense to select the 'Create Shortcuts' option (so you will find miniconda in your start menu).
4. Please follow their suggestion to not select the option of adding miniconda to your PATH variable. For now, we will not do this.


**PyCharm**

1. Go to https://www.jetbrains.com/pycharm/ and click the download button, then run the `.exe` file.
2. During installation, you have to allow PyCharm communication with local networks, but allowing access to public networks is not recommended.
3. If you open PyCharm, an interactive tutorial is opened which allows you to get to know some basic functionality. Nothing speaks against walking through this tutorial.
4. You can test if you can open a 'jupyter notebook' in PyCharm, by selecting 'New ...' or 'New File or Directory ...' from the File menu.


**Selecting the Python Interpreter in PyCharm**

1. Open PyCharm.
2. In PyCharm, go to the settings (in macOS found in the PyCharm menu entry, under windows found in the file menu). Here, select 'Python' and then 'Interpreter'. Here, please click 'Add Interpreter' -> 'Add Local Interpreter ...' and then use the file browser to select your local 'python.exe' executable file, which you find in your 'miniconda3' installation. The location of this file was determined by you during the installation of miniconda, e.g. on my computer: '~\miniconda3\python.exe'. (As you may know, the tilde '~' is a widely used shortcut that always refers to your own user directory.)
3. You can now switch between python interpreters by clicking on a drop bown menu in the status line at the bottom of the PyCharm window, which in the very right corner displays the currently used python interpreter. 

```


```{tab-item} Linux

(Note that I did not check the LINUX installation instructions as I have no LINUX machine available, but think that these should continue to work.)


**Bash shell**

You already have it!
Depending on which version of Linux you’re running you may need to type `bash` inside the terminal to access it.
To check whether this is necessary, follow these steps:

1. Open a terminal and type `echo $SHELL`.
   If it reads `/bin/bash` then you are all set!
   If not, whenever the instructions read "open a terminal," please assume you are to open a terminal, type `bash`, and then proceed with the instructions as specified.


**Python**

1. Open a new terminal and type the following lines (separately) into the terminal, pressing `Enter` after each one:

        wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
        bash Miniconda3-latest-Linux-x86_64.sh


2. A license agreement will be displayed and the bottom of the terminal will read `--More--`.
   Press `Enter` or the space bar until you are prompted with "Do you accept the license terms? [yes|no]."
   Type `yes` and then press `Enter`
3. The installation script will inform you that it is going to install into a default directory (e.g., `/home/$USER/miniconda3`).
   Leave this default and press `Enter`.
4. When you are asked "Do you wish the installer to initialize Miniconda3 by running conda init? [yes|no]," type `yes` and press `Enter`.
   Exit the terminal once the installation has finished.
5. Re-open a new terminal.
   Type `which python` into the terminal and it should return a path (e.g., `/home/$USER/miniconda3/bin/python`).
   - If you do not see a path like this then please try typing `conda init`, closing your terminal, and repeating this step.
     If your issue is still not resolved skip the following step and contact an instructor on the #help-installation channel of the BHS Slack.
6. Type the following to remove the installation script that was downloaded:

        rm ./Miniconda3-latest-Linux-x86_64.sh


**PyCharm**

1. Check whether you find PyCharm in your Linux version's packlage manager. 
2. If not, here is a description of how to install a standalone version of PyCharm under Linux: https://www.jetbrains.com/help/pycharm/installation-guide.html#standalone_linux . Often, one can also find more specific descriptions for your LINUX on the internet.
3. If you open PyCharm, an interactive tutorial is opened which allows you to get to know some basic functionality. Nothing speaks against walking through this tutorial.
4. You can test if you can open a 'jupyter notebook' in PyCharm, by selecting 'New ...' or 'New File or Directory ...' from the File menu.


**Selecting the Python Interpreter in PyCharm**

1. Open PyCharm.
2. In PyCharm, go to the settings (in macOS found in the PyCharm menu entry, under windows found in the file menu). Here, select 'Python' and then 'Interpreter'. Here, please click 'Add Interpreter' -> 'Add Local Interpreter ...' and then use the file browser to select your local 'python.exe' executable file, which you find in your 'miniconda3' installation. The location of this file was determined by you during the installation of miniconda, e.g. on my computer: '~\miniconda3\python.exe'. (As you may know, the tilde '~' is a widely used shortcut that always refers to your own user directory.)
3. You can now switch between python interpreters by clicking on a drop bown menu in the status line at the bottom of the PyCharm window, which in the very right corner displays the currently used python interpreter. 



```

```{tab-item} MacOs


**Python / Miniconda**

1. There are two ways to install miniconda on macOS - one using a graphical installer (as with many other programs), one using commandline in the terminal. Both are described on the installation page of miniconda: 

https://www.anaconda.com/docs/getting-started/miniconda/install#macos-linux-installation

The commandline installation procedures are described further down under 'quickstart'. Please note that the code given there is for newer Macs that use the Apple Silicon processors (i.e., not Intel). 

2. When using the graphical installer, you will be pointed to the download page on their website. Note: Please ignore the box on the top right that says "Download now. Get access in 30 seconds." which suggests you to register with Anaconda. Rather, go to the very bottom of the download page and click the button saying 'Download Miniconda Installer'. Here, select on the right side the correct 'Miniconda Installer' (Apple Silicon vs. Intel), download it and run it. 
3. The installation guideline webpage recommends to choose the option to install for all users, which will place the program in '/opt/miniconda3'. 


**PyCharm**

1. Go to https://www.jetbrains.com/pycharm/ and click the download button.
2. Select the *.dmg Installation image that fits to your system - either Apple Silicon or Intel processor - and download it.
3. Double click the dmg file and move PyCharm into your 'Applications' folder. 
4. If you open PyCharm, an interactive tutorial is opened which allows you to get to know some basic functionality. Nothing speaks against walking through this tutorial.
5. You can test if you can open a 'jupyter notebook' in PyCharm, by selecting 'New ...' or 'New File or Directory ...' from the File menu.


**Selecting the Python Interpreter in PyCharm**

1. Open PyCharm.
2. In PyCharm, go to the settings (in macOS found in the PyCharm menu entry, under windows found in the file menu). Here, select 'Python' and then 'Interpreter'. Here, please click 'Add Interpreter' -> 'Add Local Interpreter ...' and then use the file browser to select your local 'python.exe' executable file, which you find in your 'miniconda3' installation. The location of this file was determined by you during the installation of miniconda, e.g. on my computer: '~\miniconda3\python.exe'. (As you may know, the tilde '~' is a widely used shortcut that always refers to your own user directory.)
3. You can now switch between python interpreters by clicking on a drop bown menu in the status line at the bottom of the PyCharm window, which in the very right corner displays the currently used python interpreter. 

```
````

**Note**: If the instructions aren't working and you have spent more than 15-20 minutes troubleshooting on your own, please consider visiting the office hour offered for installation support. You will have received an email specifying when this happens. 


### Pyton Packages

For the course, we will need a few python packages that we will add to our python installation. We will do this together in the next session. 


### Preparation of your local environment

1. Please generate a folder for this course on your computer. This should be in a more or less easy to reach location (as we may have to write out the path to this folder from time to time). One possibility would be in the main folder of your account, e.g.: 

   /Users/<YourUsername>/pfp_course (macOS, LINUX) or C:\Users\<YourUsername>\ (Windows)

An alternative would be to locate this folder in your documents folder or in a folder for projects or similar: 

      /Users/<YourUsername>/Documents/pfp_course (macOS, LINUX) or C:\Users\Documents\<YourUsername>\ (Windows)

      /Users/<YourUsername>/Documents/Projects/pfp_course (macOS, LINUX) or C:\Users\Documents\Projects\<YourUsername>\ (Windows)

You can generate this folder graphically in the explorer (windows) or finder (macOS) or using the command 'md' in a bash shell or terminal (all operating systems). The most important thing is that your project folder for this course is in a location that you remember. 


2. Please download the [`environment.yml`](https://github.com/cfiebach/Python_For_Psychologists_25-26/blob/main/environment.yml) file (e.g. with right mouse click -> Save As). Make sure that the file ends with `.yml` and not `.txt`.
Please move this file your project folder. We will use this file in the next session.


### Modern web browser

Install Firefox or Chrome.
(Currently, Safari may or may not work.)
Microsoft Edge is not modern, despite what Microsoft might try and otherwise tell you.


Yeah, you did! Great job!

![logo](https://media1.tenor.com/images/d5ebabf248130ec3842ed3b8627fd4f2/tenor.gif?itemid=4770158)\
<sub><sup><sub><sup>https://media1.tenor.com/images/d5ebabf248130ec3842ed3b8627fd4f2/tenor.gif?itemid=4770158</sup></sub></sup></sub>


