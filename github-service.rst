
PythonPackages
==============

*GitHub Service Hook*

This service allows you to release Python packages from GitHub to the `Python Package Index`_, by pushing a commit message that begins with ``Release`` e.g.::

    $ git commit -a -m "Release 0.0.1" ; git push

To use the service, please follow the instructions below.

Instructions
------------

- Sign up for the pythonpackages.com beta: http://pythonpackages.com/signup.

- Follow the :ref:`introduction` instructions.

- On the Python Package Index, authorize pythonpackages.com to act on your behalf, as explained here: http://blog.aclark.net/2012/08/07/pythonpackages-com-using-pypis-oauth1-support-to-register-and-upload-packages/ (``pythonpackages.com -> Dashboard -> Manage accounts -> PyPI -> Authorize``).

- On GitHub, configure the PythonPackage service to be ``Active`` on any repository that contains a Python package you would like to release (``Repo -> Admin -> Service Hooks -> PythonPackages -> [*] Active``).

Now you can git push to release! If you have any trouble, please _`open a ticket`.

.. _`open a ticket`: https://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

.. _`Python Package Index`: https://pypi.python.org/pypi
