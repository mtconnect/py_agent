py_agent
========

### Just getting started w/ Python Agent

So we're going to try to use Flask for the Python Agent. Flask is a microframework for Python based on Werkzeug and Jinja 2. Flask depends on two external libraries, Werkzeug and Jinja2. Werkzeug is a toolkit for WSGI, the standard Python interface between web applications and a variety of servers for both development and deployment. Jinja2 renders templates. So how do we get all that installed simply and quickly. There are a couple ways to do this, but probably the best way is to do a virtualenv(virtual environment). Most of the information described can be found on the Flask docs site.

###virtualenv

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

