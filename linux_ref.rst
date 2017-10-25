Linux Terminal Basics
=====================

Just make sure you know all these before heading into this, you'll use them constantly in Git Bash.

Navigation Commands
-------------------

Here is a list of commands you need to know to move through the file system structure in Bash

* ``pwd`` Shows your present working directory
* ``ls`` lists all the directories in your present working directory
* ``cd directory_name`` moves into a folder named directory_name, making it your present working directory
* ``cd ..`` goes back a level *ie: to leave directory_name and return to your root directory*

Make and Delete Folders
-----------------------

Since you're already looking at a terminal window and want to stay on track, it's best to know how to make and delete directories.

* ``mkdir directory_name`` this makes an empty folder in your present working directory called directory_name
* ``rm -rf directory_name`` this forcefully deletes a folder in your present working directory called directory_name and all of its contents

Doing the thing for the first time
----------------------------------

Wade is probably the only person who will need to look at this section, but it's here for reference anyway

Install backend
1. ``apt-get install pip``
2. ``sudo pip install Sphinx``
3. ``sudo pip install sphinx_rtd_theme``

Start a new template
1. Navigate to a folder you want the new document to be in and run ``sphinx-quickstart`` defaults should work just fine.
2. Edit conf.py ``html_theme = 'sphinx_rtd_theme'``
3. initial build ``make html``

Start Tracking with Git
1. in the project's directory ``git init``
2. confirm git was made with ``ls -a``
3. add all the files with ``git add .``
4. commit to the local repo ``git commit -m "initial commit"``
5. make github repo without readme at github.com
6. link the repo to the local git ``git remote add origin [address listed]``
7. initial push ``git push -u origin master``

Link to Readthedocs
1. Import a Project
2. Find on list populated from github
3. Clone the repo to a work computer and work on that shit
