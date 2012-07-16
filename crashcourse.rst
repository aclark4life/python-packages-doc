
.. Note:: The beta release features are intended for use by anyone who `signs up for the beta`_. pythonpackages.com checks your GitHub email address against your beta signup email address. However, the GitHub API currently only returns an email address if you've configured one to display publicly here: https://github.com/settings/profile. If you have signed up for the beta (before July 9 2012, afterwards the form requires your GitHub username) but don't want to display your email to the public, please `open a ticket`_ and include your GitHub username. We will then whitelist your account.
    :class: alert alert-info

Crash course (for beta users)
=============================

Welcome. Please follow the steps in this guide to get started using pythonpackages.com beta release features.

Step 1: Access
--------------

* Sign up for the beta if you haven't already.

* Login with your GitHub Account.

* Select Username -> Dashboard. You should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/crashcourse.png

Step 2: Add package slot and select repository
----------------------------------------------

* With the free plan, you have access to a single package slot. You can use this slot to select any repository in your GitHub account.

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/crashcourse2.png

* Now select a repository that contains a Python package you would like to release.

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/crashcourse2-1.png

Step 3: Test release
--------------------

* Warning: there is no magic yet. In addition to selecting a valid package, you should add a `MANIFEST.in file`_ if you don't have one already. pythonpackages.com does not know about any version control integration you may be using locally.

* Send the release to the test index server with the "Test release" button. You should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/crashcourse3.png

Please report any issues you encounter here:

* https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

Thank you for using the beta release features. Once you feel comfortable using the system, you are welcome to release your packages to PyPI by pressing the "Release" button. This will create a release tag for you on GitHub via your last commit. A lot more features and task automation are being planned, but first we need your help to test and stablize the beta release.

.. _`MANIFEST.in file`: http://docs.python.org/distutils/sourcedist.html#the-manifest-in-template

.. _`open a ticket`: https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

.. _`signs up for the beta`: https://pythonpackages.com/signup
