.. include:: section-note.rst

Background
==========

Perhaps one of the most challenging concepts to explain to beginners and highly
skilled programmers alike is how to install Python software (including
Python itself!) Assuming the subject is someone with basic computer literacy, who 
understands the concept of "installers", then you might tell him or her to::

    "Go to python.org, then download and run the installer!"

Everything that happens after that, from writing and running
your first *hello_world.py* program to deploying your sophisticated web
application on heroku.com, is an extension of this basic concept. You have a
**computer** (i.e. your development laptop, or production workstation, or nebulous
cloud application environment) and you want to run **software** on it.


Python and its available libraries
----------------------------------

We aren't going to cover the installation of Python here. But suffice it to say, one
uses either a *binary installer* or a *compiler* to build the *source code*.
If you use an installer, sometimes that installer may let you install additional
packages that are not distributed with Python itself::

    $ aptitude install python2.7-biopython


If you are able to do this, it is a happy day! But sometimes the
software or version of software we want is not distributed via this method.
By installing additional "installers", you can gain access to over 18,000
packages from the Python Package Index!


Available installers
--------------------

We aren't going to cover *distutils*, or *setuptools* and it's popular fork
called *distribute*. Nor are we going to cover *distutils2* and Python 3's
*packaging* library. What we *are* going to cover is this: **Python provides
its own set of tools for installing Python software** (in addition to your operating
system's package manager) which you may find useful. One such tool is called
``pip``.

``pip`` Installs Packages
~~~~~~~~~~~~~~~~~~~~~~~~~

Perhaps you have used your operating system's package manager to install
``pip``.
Or perhaps you have installed it some other way. We aren't going to cover
installation of ``pip`` here, but we are going to tell you it allows you to do
things like this::

    $ pip install Django


``easy_install`` installs packages too
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

``easy_install`` is part of *setuptools* (and subsequently *distribute*) and is
much older than ``pip`` and much less featureful. However, if it is available
on your system (and if you have installed *setuptools* or *distribute*, it is) you
may use it like so::

    $ easy_install Django

Just keep in mind it may become less available in the future.


``buildout`` installs packages three, using ``easy_install``
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Unlike ``easy_install`` or ``pip``, ``buildout`` requires the creation of a configuration
file in order to install packages with it. In exchange (if you will) it offers a
plugin system to allow you to install just about any software, or perform just
about any configuration task. It does this by supporting *ini-style*
configuration on top of ``easy_install``, as well as supporting plugins via
another ``setuptools`` feature: *entry points*. We will not explain those here,
but simply put: any Python package may declare itself a buildout "recipe", and
provide whatever functionality it likes.

``Pyg`` installs packages four
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The newest installer to join the group is ``Pyg``. According to its
documentation::

    Pyg is a Python Package Manager that is meant to be an alternative to
    easy_install and Pip. It can install, remove, bundle Python packages and much
    more.

See: http://pythonpackages.com/info/pyg for more information.

Prophylactics
-------------

Lastly, we will mention this: due to Python internals, only a single version of
a Python module may exist in any given Python installation at run time. As such,
various tools have been developed over the years to work around this limitation.
One such tool is ``virtualenv``.

Virtualenv
~~~~~~~~~~

To put it better, from the ``virtualenv`` documentation::

    The basic problem being addressed is one of dependencies and versions, and
    indirectly permissions. Imagine you have an application that needs version 1 of
    LibFoo, but another application requires version 2. How can you use both these
    applications? If you install everything into /usr/lib/python2.7/site-packages
    (or whatever your platform's standard location is), it's easy to end up in a
    situation where you unintentionally upgrade an application that shouldn't be
    upgraded.

So you will often see ``virtualenv`` mentioned during a discussion of package
installation. Keep in mind that the use of ``virtualenv`` is primarily a
prophylactic measure. If you do not know whether you need it or not, it cannot
hurt:: 

    $ pip install virtualenv
    $ virtualenv <ENV>
    $ cd <ENV>
    $ bin/pip install <PACKAGE>

Buildout
~~~~~~~~

To some extent, ``buildout`` is a tool you can use to take similar prophalactyc
measures. That is because it downloads and installs packages to a neutral
location then provides scripts to load them, all in complete isolation from the
"parent" Python installation.

But that is not its only purpose, and in some cases you may benefit from using
a ``virtualenv`` "in between" a buildout and its "parent" Python installation::

    $ virtualenv .
    $ bin/pip install zc.buildout
    $ bin/buildout init

This brings us to our first example.

.. include:: disqus.html
