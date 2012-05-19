.. include:: note-about-build-section.rst

Example #1 - Jenkins
====================

That was along way to go explain the following: we have some ready made
configuration files available for you to use with ``buildout`` (and ``pip``,
coming soon).

Continous integration with ``Jenkins``
--------------------------------------

You are developing some Python software and you would like to begin automated,
continuous integration testing. You know that in production you may do
something completely different to meet your continuous integration needs,
but for now you just want something quick and dirty to get started.
``java`` has been installed already, by your operating
system's package manager. You type::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Then edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://pythonpackages.com/buildout/jenkins/1.464

Then run::

    $ bin/buildout

Followed by::

    $ bin/supervisord -e debug -n

At which point you should see::

    2011-12-21 18:58:21,021 DEBG 'jenkins' stderr output:
    Dec 21, 2011 6:58:21 PM hudson.WebAppMain$2 run
    INFO: Jenkins is fully up and running

Open the following URL in your web browser:

 - http://127.0.0.1:8080

And you should see:

.. image:: https://github.com/aclark4life/pythonpackages-docs/raw/master/ex1-jenkins-00.png
    :width: 336.5
    :height: 240.5

Happy times!

.. include:: disqus.html
