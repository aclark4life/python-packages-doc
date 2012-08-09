
GitHub Service
==============

This service allows you to release Python packages from GitHub to the Python Package Index, simply by pushing a commit message that begins with ``Release`` e.g.::

    $ git commit -a -m "Release 0.0.1"

To use the service, please follow the instructions below.

Instructions
------------

- Sign up for the pythonpackages.com beta here: http://pythonpackages.com/signup.

- Follow the :ref:`introduction` instructions.

- On GitHub, configure the PythonPackage service to be ``Active`` on any repository that contains a Python package you would like to release (Repo -> Admin -> Service Hooks -> PythonPackages -> [*] Active).
- 
