# Python Interpreter

You have several options for getting a version of python. You'll find that everyone and their mother has an opinion on best practices for installing python. However, for the sake of this workshop we will simplify the options to two: (1) the barebones version from [python.org](http://python.org) where you can install your own python packages, and (2) the all in one package made available by Continuum Analytics. There are also other ways to install python depending on your operating system that you may hear of including brew, apt-get and so on (see the notes section below).

###Python

**Option 1, cleanest install**
The current production versions are Python 2.7.5 and Python 3.3.2. For barebones python installation, go to [http://python.org/download/](http://python.org/download/) and download the source file. 

**Option 2, one step process**
If you would like to use Python for scientific computing, you may wish to consider [Anaconda](https://store.continuum.io/cshop/anaconda/). The [fine print](http://docs.continuum.io/anaconda/pkgs.html) says you'll need to install [conda](http://docs.continuum.io/conda/index.html) to have Python 3.3.2.

**Option 3**
Vagrant set up - we're in the process of creating a set up file so that all you have to do is type in `vagrant up`

Having python interpreter lets you compile the python code into something that your machine can run. It is necessary for any files with the *.py extension!

**Python 2 vs Python 3**
We're going to suggest that you go with python2 for now because it's the most commonly used, but refer to [this guide](https://wiki.python.org/moin/Python2orPython3) for the differences between the two.

* [Python 3 wall of superpowers](http://python3wos.appspot.com/) - see which packages have been ported to python3

###Development tools

We're introducing here a couple of commonly used tools for development workflow: (1) package manager, making it easy to install and uninstall packages and (2) virtual environments to make it easier to work on more than one project at a time without introducing conflicts in their dependencies.

*Note* on a mac, you would install pip with `sudo easy_install pip` and then install virtualenv with `pip install virtualenv, virtualenvwrapper`

* [Python Package Index](https://pypi.python.org/pypi/pip) - it is a manager that helps you keep track of python packages.
* [VirtualEnv](http://virtualenv.readthedocs.org/) - virtualenv is a tool to create isolated Python environments
* [VirtualEnvWrapper](http://virtualenvwrapper.readthedocs.org/) a set of extensions for creating and deleting virtual environments and otherwise managing your development workflow, making it easier to work on more than one project at a time without introducing conflicts in their dependencies.


**NOTE**

Mac OSX users may need to install the [command line tools](https://developer.apple.com/downloads/index.action?=command%20line%20tools) to use certain packages (free developer account required). You may also prefer using [macbrew](http://brew.sh/). Some people use something called [macports](http://www.macports.org/), though be aware that it does not work well with macbrew together.

Debian based linux users can use [apt-get](https://wiki.debian.org/apt-get) for installing pip. 


##FAQ

*Doesn't *nix systems come defult with Python?*

Which versions of Python are available will differ based on the package manager as well as the OS version. For example, Ubuntu 12.04 only goes up to 3.2 without adding an additional package archive (called deadsnakes). On 12.10 and newer, it may be listed as python3 and not python3.3.

*I've seen people use apt-get for installations before, couldn't I use that?*

Debian-based linux distribusions use aptitude (apt-get). Others (e.g., RedHat, Fedora, CentOS) use yum. People often report having issues after installing python via homebrew or macports, so the general recommendation is to install directly from python.org

*Where can I learn more about python version 2 and 3?*

There was a talk on this topic earlier this year by Julian Berman, on [The Ups and Downs of Migrating to Python 3: A Pragmatic Approach](http://www.meetup.com/nylug-meetings/events/82181832/). You can look in the comments section for slides to his talk.

