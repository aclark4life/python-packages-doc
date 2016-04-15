.. _introduction:

Introduction
============

Welcome. pythonpackages.com helps Python programmers package and release their software with just a few clicks. To get started, please follow the steps below:

Access
------

- Sign up for the beta (if you haven't already): http://pythonpackages.com/signup.
- Sign in to pythonpackages.com with your GitHub account.
- View your dashboard:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction1.png
  :class: thumbnail

- You are now using the free plan.

Package slot
------------

- The free plan provides access to a single package slot, which you may use to select any repository from your personal GitHub account. (You may select/unselect a single repository an  unlimited number of times. However, if you use the service regularly to manage more than a single package and/or you want to manage an Organization's repository, please consider purchasing one of the `paid plans`_.)

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction2.png
  :class: thumbnail

Select repository
-----------------

.. Warning:: pythonpackages.com does not know about any version control system integration tools you may be using locally e.g. `setuptools-git`_, so the package you select must contain a properly configured `MANIFEST.in file`_, otherwise you may inadvertently create a `brown bag`_ release.
  :class: alert alert-warning 

- Now select a repository that contains a Python package you would like to test and release.

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction3.png
  :class: thumbnail

Test release
------------

- Now press the "Test release" button to send your package to the `test index server`_. You should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction4.png
  :class: thumbnail

At this point, you can perform additional testing using the test index e.g.::

    $ pip install PACKAGE -i http://index.pythonpackages.com

Release
-------

Once you are confident everything works as expected, release your package to PyPI by pressing the "Release" button. This will create a release tag for you on GitHub based on your last commit. (You can also refer `create-packages <https://github.com/pythonpackages/documentation/blob/master/create-package.rst/>`_.)

Report bugs
-----------

Please report any issues you might encounter here:

- https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

.. _`MANIFEST.in file`: http://docs.python.org/distutils/sourcedist.html#the-manifest-in-template

.. _`open a ticket`: https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

.. _`signed up for the beta`: http://pythonpackages.com/signup

.. _`paid plans`: http://pythonpackages.com/plans

.. _`test index server`: http://index.pythonpackages.com

.. _`brown bag`: http://guide.python-distribute.org/specification.html#pre-releases

.. _`setuptools-git`: http://pythonpackages.com/package/setuptools-git

.. include:: disqus.html
