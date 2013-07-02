runmycode.github.io
====================

http://runmycode.github.io

This is the developer team page for RunMyCode.

The pelican code in the ''pelicansrc'' branch publishes code to the ''master'' branch.

To set up the site dev environment for the first time, get the src and install dependencies.

* check out this repo by running `git clone git@github.com:runmycode/runmycode.github.com.git`
* cd to the repo by typing `cd runmycode.github.com`
* checkout the pelicansrc branch
* create a virtualenv by typing `virtualenv venv`
* activate the virtualenv by typing `source venv/bin/activate`
* install python requirements by typing `pip install -r requirements.txt`

To work on the site once you've got the dependencies installed

* be in the repo directory
* source venv/bin/activate
* be in the pelicansrc branch
* Write new content
 * `make devserver`, make sure you like the results
 * `make stopserver`, once you are done looking at the results
* check your changes in to the source branch
* generate changes for the master branch:
 * `make html`
 * `make github`

The github target pushes the generated pages to the master branch which github
will detect and publish.
