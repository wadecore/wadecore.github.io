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

Using Sphinx
------------

Wade is probably the only person who will need to look at this section, but it's here for reference anyway

Install backend
#. ``apt-get install pip``
#. ``sudo pip install Sphinx``
#. ``sudo pip install sphinx_rtd_theme``

Start a new template
#. ``sphinx-quickstart``
#. Edit conf.py ``html_theme = 'sphinx_rtd_theme'``
