.. include:: note-about-build-section.rst

Example #2
==========

And now for a familiar topic, Apache and mod_wsgi.

``Apache`` with "hello world" WSGI app
--------------------------------------

You want to understand how to set up your WSGI application under mod_wsgi. You decide
to run the simplest possible application locally in order to see how it works::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Then edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://build.pythonpackages.com/buildout/apache/latest

Then run::

    $ bin/buildout

Followed by::

    $ bin/supervisord -e debug -n

At which point you should see::

    2011-12-22 14:54:00,083 DEBG 'apache' stdout output:
    [Thu Dec 22 14:54:00 2011] [notice] Apache/2.2.21 (Unix) mod_ssl/2.2.21
    OpenSSL/0.9.8r DAV/2 mod_wsgi/3.3 Python/2.7.2 configured -- resuming normal
    operations

Open the following URL in your web browser:

 - http://127.0.0.1:8080

And you should see:

.. image:: https://github.com/aclark4life/pythonpackages-docs/raw/master/ex2-apache-00.png

Happy times!

.. include:: disqus.html
