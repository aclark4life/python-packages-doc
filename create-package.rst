
.. _create-packages:

Create packages
===============

In addition to testing and releasing existing packages, you can also create new packages with pythonpackages.com.

PasteScript
-----------

There is a venerable Python library called ``PasteScript`` which lets you execute commands like this::

    $ paster create -t basic_package my_app

This command creates a Python package for you. Otherwise you'd have to do something like::

    $ mkdir -p my_app/my_app
    $ touch my_app/setup.py
    $ touch my_app/my_app/__init__.py

In addition to the core templates provided by PasteScript, there are many add-on templates available for almost any kind of Python project you can think of.

Through the web
~~~~~~~~~~~~~~~

pythonpackages.com is PasteScript through the web. To use it, sign in and select ``Create new package`` from the ``Manage packages`` section. Select a template and enter a package name, then submit via the ``Create`` button.

.. Note:: If you have not entered them, you will be `prompted for your GitHub credentials`_.
  :class: alert

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/create-package1.png
   :class: thumbnail

View results
------------

Wait for the results.

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/create-package2.png
   :class: thumbnail

Now check GitHub.

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/create-package3.png
   :class: thumbnail

.. _`prompted for your GitHub credentials`: http://docs.pythonpackages.com/en/latest/security.html
