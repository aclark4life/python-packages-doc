
Introduction
============

Welcome. Please follow these steps to start using the pythonpackages.com beta release features.

Step 1: Access
--------------

- Sign up for the beta, if you haven't already: http://pythonpackages.com/signup.

- Sign in to pythonpackages.com with your GitHub account.

- You should be redirected to your dashboard, where you should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/intro.png

Step 2: Add package slot and select repository
----------------------------------------------

- With the free plan, you have access to a single package slot. You can use this slot to select any repository in your GitHub account.

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/intro2.png

- Now select a repository that contains a Python package you would like to release.

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/intro3.png

Step 3: Test release
--------------------

.. Warning:: There is no VCS integration

- In addition to selecting a valid package, you should add a `MANIFEST.in file`_ if you don't have one already. pythonpackages.com does not know about any version control integration you may be using locally.

- Send the release to the test index server with the "Test release" button. You should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/intro4.png

Please report any issues you encounter here:

- https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

Thank you for using the beta release features. Once you feel comfortable using the system, you are welcome to release your packages to PyPI by pressing the "Release" button. This will create a release tag for you on GitHub via your last commit.

.. _`MANIFEST.in file`: http://docs.python.org/distutils/sourcedist.html#the-manifest-in-template

.. _`open a ticket`: https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

.. _`signed up for the beta`: https://pythonpackages.com/signup
