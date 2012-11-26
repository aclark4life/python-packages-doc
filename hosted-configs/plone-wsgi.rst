.. Note:: `View config on GitHub`_
  :class: alert alert-info

Plone + WSGI
============

You understand deploying Plone via WSGI is not yet fully supported (or functional), but you still want to take a WSGI-powered ``Plone`` for a spin::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = https://raw.github.com/pythonpackages/buildout-plone/master/4.3.x-wsgi

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

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/hosted-configs/plone1.png
   :class: thumbnail

.. include:: ../disqus.html

.. _`View config on GitHub`: https://github.com/pythonpackages/buildout-plone/blob/master/4.3.x-wsgi
