# End to End Machine Learning Project

### Agenda:

1. Set up github
    - new environment
    - setup.py
    - requirements.txt
2. src folder and build the package


## Create repo

Create empty repo in github


## Setup venv

Create folder and open in vs code. In that folder, create virtual environment.

```
conda create -p venv python==3.8 -y

conda activate venv
```

## First commit in repo

From terminal in local:

Init git repo

```
git init
```

Create and add readme file

```
git add README.md
git commit -m "First commit"
```


Connect local repo with github. when you create an empty repo in github, it shows you this code to connect.
Make sure before push that you have git.config updated with email.

```
git branch -M main
git remote add origin https://github.com/josrodand/mlproject.git
git push -u origin main

```

## Create .gitignore file 

You can do this from github. select create new file an write .gitignore. Select python as language and file will be filled automatically.

Make a commit from github and add .gitignore.

After that, you have to make a pull in local

```
git pull
```

This process can be automated. later on.

## setup.py

This allows to create our machine learning model as a package. You will make updates and install this package in our projects.
After that you will upload your package in pypl. 

## create src

Create src folder and `__init__.py` file

## create requirements.txt

Put all needed modules. You can put `-e .` at the end to help setup.py to install al requirements.

After that, install requirements

```
pip install -r requirements.txt
```

Having  `-e .` in requirements file will do that instalation connects with setup.py and will create a package metadata folder: ``mlproject.egg-info``
