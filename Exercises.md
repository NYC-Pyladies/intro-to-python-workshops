# Exercises for Intro to Python 1: Setting up your development environment

Try these exercises to test your understanding of python installation and working from the command line. Here are some examples for reference.

```
# Checking Python version 
$ python --version

# Checking path to Python interpreter
$ which python

# Starting a virtual environment. 
# Creating a virtual environment will automatically drop you into it.
$ mkvirtualenv yourvirtualPython2

# Closing virtual environment 
(yourvirtualPython2)$ deactivate

# Installing a virtualenv with Python3 
$ mkvirtualenv -p 'which python3' yourvirtualPython3

# List of virtual environments 
$ workon

# Activating a virtual environment
$ workon yourvirtualPython2

# Deleting a virtual enviroment
$ rm -rf yourvirtualPython2

# Saving list of packages into a file 
$ pip freeze > requirements.txt

# previewing a text file
$ cat requirements.txt
```

## Exercise 1

Create a virtual environment named *TheHolyGrail* with Python3
- Install these packages Flask, sqlalchemy, flask-sqlalchemy
- Work on *TheHolyGrail*
- Save the list of installed packages into a file named 'requirements.txt'
- Exit the virtual environment
 
## Exercise 2 

Create a virtual environment named *KungFu*
- Install these packages Python 2, pandas
- Work on *KungFu*
- Save the list of installed packages into a file named 'requirements.txt'
- Exit the virtual environment

To preview the requirements file from the command line, you can type in the bash command `cat requirements.txt`
