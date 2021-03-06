GitGitLab: Gitlab Git Plugin
============================

GitGitLab allows you to create Gitlab projects and set them as remote source for your git checkouts.


Installation
------------

.. code::

	sudo pip install gitgitlab


Usage
-----

.. code::

	$ git init
	$ git touch 'readme.txt'
	$ git add readme.txt
	$ git commit -am 'initial commit'
	$ git lab create my_project -t
	  Project my_project created on Gitlab
	$ git remotes
	  gitlab


Command overview
----------------

**git lab list**
	List your Gitlab projects
**git lab create <project name>**
	Create a project on Gitlab
**git lab track <project name>**
	Set this project as remote for your local repository.
**git lab open <project name>**
	Open a Gitlab project page. If <project name> is omitted, uses the project on the 'gitlab' remote of the repository on the current directory.

Listing your projects
----------------------

**git lab list** lists all the projects that you own and their repository url.

Creating a new project
----------------------

**git lab create <project_name>** creates a new private project on Gitlab.

**git lab create <project_name> --track** creates a new private project and sets it up as remote.

Setting up an existing project to track the local repository
------------------------------------------------------------

**git lab track <project_name>** Adds a gitlab project as remote.

Obtaining help
--------------

**git lab help**
	Overview.
**git lab <command> --help**
	Help for a specific command.

More information
----------------

See also the `project documentation <http://gitgitlab.readthedocs.org>`_.
