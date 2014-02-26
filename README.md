py_agent
========

### Just getting started w/ Python Agent

So we're going to try to use Flask for the Python Agent. Flask is a microframework for Python based on Werkzeug and Jinja 2. We'll also be using Flask-RESTful an extension to Flask. Obviously this is all subject to change, but this can be a good start for the Python Agent. Flask depends on two external libraries, Werkzeug and Jinja2. Werkzeug is a toolkit for WSGI, the standard Python interface between web applications and a variety of servers for both development and deployment. Jinja2 renders templates. So how do we get all that installed simply and quickly. There are a couple ways to do this, but probably the best way is to do a virtualenv(virtual environment). Most of the information described can be found on the Flask docs site.

###virtualenv and installing Flask

Virtualenv enables multiple side-by-side installations of Python, one for each project. It doesn’t actually install separate copies of Python, but it does provide a great way to keep different project environments isolated. See below how a virtualenv works.

If you are on Mac OS X or Linux, chances are that one of the following two commands will work for you:

```
$ sudo easy_install virtualenv
```

or

```
$ sudo pip install virtualenv
```

One of these will probably install virtualenv on your system. Maybe it’s even in your package manager. If you use Ubuntu, try:

```
$ sudo apt-get install python-virtualenv
```

If you are using Windows please scroll down to the Windows Users section to see how to install.

Once you have the virtualenv installed, open up terminal (aka a shell) and create your own environment. You can create a project folder then a venv folder within that folder:

```
$ mkdir myproject
$ cd myproject
$ virtualenv venv
New python executable in venv/bin/python
Installing distribute............done.
```

Ok, whenever you want to work on a project, you only have to activate the corresponding environment. On OS X and Linux, do the following:

```
$ . venv/bin/activate
```

If you are a Windows user, use the following command:

```
$ venv\scripts\activate
```

Now, you should now be using your virtualenv (notice how the prompt of your shell has changed to show the active environment).

Now you can just enter the following command to get Flask activated in your virtualenv:

```
$ pip install Flask
```

And there you go, at least with getting Flask installed. Next we'll need to install Flask-RESTful.

###installing Flask-RESTful

Install Flask-RESTful with pip

```
pip install flask-restful
```

Flask-RESTful has the following dependencies (which will be automatically installed if you use pip):

Flask version 0.8 or greater
Flask-RESTful requires Python version 2.6, 2.7, or 3.3.

Now, after all that is done, we are ready to start the Agent. To do this make sure you are in the project folder that we created above and make sure you have activated your virtual environment. Now run the command below:

```
python agent.py
```

There you have it! Your agent should be running at 127.0.0.1:5000 (aka http://localhost:5000)

###Windows Users

On Windows, installation of easy_install is a little bit trickier, but still quite easy. The easiest way to do it is to download the distribute_setup.py file and run it. The easiest way to run the file is to open your downloads folder and double-click on the file.

Next, add the easy_install command and other Python scripts to the command search path, by adding your Python installation’s Scripts folder to the PATH environment variable. To do that, right-click on the “Computer” icon on the Desktop or in the Start menu, and choose “Properties”. Then click on “Advanced System settings” (in Windows XP, click on the “Advanced” tab instead). Then click on the “Environment variables” button. Finally, double-click on the “Path” variable in the “System variables” section, and add the path of your Python interpreter’s Scripts folder. Be sure to delimit it from existing values with a semicolon. Assuming you are using Python 2.7 on the default path, add the following value:

```
;C:\Python27\Scripts
```

And you got it! To check that it worked, open the Command Prompt and execute easy_install. If you have User Account Control enabled on Windows Vista or Windows 7, it should prompt you for administrator privileges.

Now that you have easy_install, you can use it to install pip:

```
> easy_install pip
```
