
Introduction
============

Welcome. Please follow these steps to get started testing the pythonpackages.com beta release features.

Step 1: Access
--------------

- Sign up for the beta, if you haven't already: http://pythonpackages.com/signup.

- Sign in to pythonpackages.com with your GitHub account.

- You should be redirected to your dashboard, where you should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction.png
  :class: thumbnail

Step 2: Add package slot
------------------------

- With the free plan you have access to a single package slot, which you may use to select a repository from your personal GitHub account. (You may select/unselect a single repository an  unlimited number of times. However, if you use the service regularly for more than a single package and/or you need access to a GitHub organization repository, please consider purchasing one of the `paid plans`_.)

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction2.png
  :class: thumbnail

Step 3: Select repository
-------------------------

- Now select a repository that contains the Python package you would like to release.

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction3.png
  :class: thumbnail

Step 4: Test release
--------------------

.. Warning:: There is no version control system integration
  :class: alert alert-warning

- In addition to selecting a valid package, you should add a `MANIFEST.in file`_ if you have not done so already. pythonpackages.com does not know about any version control integration you may be using locally e.g. setuptools-git.

- Send the release to the test index server with the "Test release" button. You should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/introduction4.png
  :class: thumbnail

Please report any issues you encounter here:

- https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

Thank you for using the beta release features. Once you feel comfortable using the system, you are welcome to release your packages to PyPI by pressing the "Release" button. This will create a release tag for you on GitHub via your last commit.

.. _`MANIFEST.in file`: http://docs.python.org/distutils/sourcedist.html#the-manifest-in-template

.. _`open a ticket`: https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

.. _`signed up for the beta`: https://pythonpackages.com/signup

.. _`paid plans`: http://pythonpackages.com/plans
