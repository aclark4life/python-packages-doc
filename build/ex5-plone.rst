.. include:: note-about-build-section.rst

Example #5
==========

The award-winning, Python-based, Plone CMS.


WSGI-powered ``Plone`` setup
----------------------------

You want to take a WSGI-powered ``Plone`` for a spin::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://build.pythonpackages.com/buildout/plone/4.2.x

Then run::

    $ bin/buildout

Followed by::

    $ bin/paster serve plone.ini

At which point you should see::

    Starting server in PID 51320.
    serving on http://127.0.0.1:8080

Open the following URL in your web browser:

 - http://127.0.0.1:8080

You should see:

.. image:: https://github.com/aclark4life/pythonpackages-docs/raw/master/plone.png

Happy times!

.. include:: disqus.html
