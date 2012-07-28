
.. _create-packages:

Create packages
===============

In addition to testing and releasing your existing packages, pythonpackages.com can help you create new packages.

PasteScript
-----------

There is a venerable Python library called ``PasteScript`` which lets you execute commands like this::

    $ paster create -t basic_package my_app

This command creates the files and directories of a Python package for you. Otherwise you'd have to do something like this::

    $ mkdir -p my_app/my_app
    $ touch my_app/setup.py
    $ touch my_app/my_app/__init__.py

In addition to the core templates provided by PasteScript, there are add-on templates available for almost any kind of Python project you can think of.

Through the web
~~~~~~~~~~~~~~~

You can think of pythonpackages.com as "PasteScript through the web". To use it, sign in and select ``Create new package`` from the ``Manage packages`` section. Then select a template and enter a package name. Then press the ``Create`` button.

.. Note:: If you have not entered them, you will be `prompted for your GitHub credentials`_.
  :class: alert

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/create-package1.png
   :class: thumbnail

Results
-------

Now wait (a few seconds) for the results.

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/create-package2.png
   :class: thumbnail

These results indicate your package has been created on GitHub. You can verify this by signing in to GitHub to check for the new package.

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/create-package3.png
   :class: thumbnail

Test and release
----------------

You can now test and release your new package, as described in the :ref:`introduction`.

.. _`prompted for your GitHub credentials`: http://docs.pythonpackages.com/en/latest/security.html
