.. include:: section-note.rst

Example #1
==========

That was along way to go explain the following: we have some ready made
configuration files available for you to use with ``buildout``. We are also
planning to host useful sets of ``pip`` requirements.txt files, though ``pip``
currently does not support network transfer of such files, therefore the
current usefulness of doing that is dubious. Until then, and until we have time
to explain more about the complete set of ``buildout`` configuration files
currently available, please consider the following example.

Continous integration with Jenkins
----------------------------------

You are developing some Python software and you would like to begin automated,
continuous integration testing. You know that in production you may do
something completely different to meet your continuous integration needs,
but for now you just want something quick and dirty to get started.
``java`` has been installed already, by your operating
system's package manager. You type::

    $ virtualenv .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Then you edit the contents of buildout.cfg to include::

    [buildout]
    extends = http://build.pythonpackages.com/buildout/jenkins/latest

Then you run::

    $ bin/buildout

Followed by::

    $ bin/supervisord -e debug -n

At which point you see::

    2011-12-21 18:58:21,021 DEBG 'jenkins' stderr output:
    Dec 21, 2011 6:58:21 PM hudson.WebAppMain$2 run
    INFO: Jenkins is fully up and running

So you open the following URL with your web browser:

 - http://127.0.0.1:8080

And you see:

.. image:: https://github.com/aclark4life/pythonpackages-docs/raw/master/jenkins.png

Happy times! Stay tuned for more.
