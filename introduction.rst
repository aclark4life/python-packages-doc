
Introduction
============

Welcome. Please follow the steps below to test the beta release features.

Step 1: Get access
------------------

- Sign up for the beta, if you haven't already: http://pythonpackages.com/signup.
- Sign in to pythonpackages.com with your GitHub account.
- You should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction.png
  :class: thumbnail

Step 2: Add package slot
------------------------

- The free plan provides access to a single package slot, which you may use to select any repository from your personal GitHub account. (You may select/unselect a single repository an  unlimited number of times. However, if you use the service regularly to manage more than a single package and/or you want to manage an Organization's repository, please consider purchasing one of the `paid plans`_.)

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction2.png
  :class: thumbnail

Step 3: Select repository
-------------------------

.. Warning:: There is no version control system integration. In addition to selecting a valid package, you must add a properly configured `MANIFEST.in file`_ (if you haven't already). pythonpackages.com does not know about version control integration e.g. setuptools-git and without a properly configured MANIFEST.in file you may create a `brown bag`_ release.
  :class: alert alert-warning 

- Now select a repository that contains a Python package you would like to test and release.

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction3.png
  :class: thumbnail

Step 4: Test release
--------------------

- Now press the "Test release" button to send your package to the `test index server`_. You should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction4.png
  :class: thumbnail

Step 5: Have fun and profit
---------------------------

Thank you for testing the beta release features. Once you feel comfortable, please release your package to PyPI by pressing the "Release" button. This will create a release tag for you on GitHub based on your last commit. Please report any issues you may encounter here:

- https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

.. _`MANIFEST.in file`: http://docs.python.org/distutils/sourcedist.html#the-manifest-in-template

.. _`open a ticket`: https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

.. _`signed up for the beta`: https://pythonpackages.com/signup

.. _`paid plans`: http://pythonpackages.com/plans

.. _`test index server`: http://index.pythonpackages.com

.. _`brown bag`: http://guide.python-distribute.org/specification.html#pre-releases
