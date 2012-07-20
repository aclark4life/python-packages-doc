.. include:: note-about-build-section.rst

Example #5 - WSGI-powered Plone
===============================

The award-winning, Python-based, Plone CMS. You want to take a WSGI-powered ``Plone`` for a spin::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://pythonpackages.com/buildout/plone/4.2.x-wsgi

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

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/features/hosted-configs/ex5-plone-00.png
   :width: 294
   :height: 187

Happy times!

.. include:: disqus.html
