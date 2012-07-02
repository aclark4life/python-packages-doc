
Crash course for beta users
===========================

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

* Beware there is no magic yet. In addition to selecting a working package, you should add a MANIFEST.in file to your package if you have not done so already. pythonpackages.com does not know about any version control integration you may be using locally.

* Send the release to the test index server with the "Test release" button. You should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/crashcourse3.png

Please report any issues you encounter here:

* https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

Thank you for using the beta relase features. Please feel free to release packages to PyPI by pressing the "Release" button, once you feel comfortable using the system. This will automatically create a release tag for you on GitHub from your last commit. A lot more features and task automation are being planned, but we need your help to test and stablize the beta release first.
