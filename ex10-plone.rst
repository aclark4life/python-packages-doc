.. include:: note-about-build-section.rst

Example #10 - Plone
===================

The award-winning, Python-based, Plone CMS. This time with the supported
Python 2.6 and ZServer (instead of Python 2.7, which will be supported soon and
WSGI, whose support has yet to be determined.)


Supported ``Plone`` setup
-------------------------

You want to take ``Plone`` for a spin::

    $ virtualenv-2.6 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://pythonpackages.com/buildout/plone/latest

Then run::

    $ bin/buildout

Followed by::

    $ bin/plone fg

At which point you should see::

    2012-01-09 19:53:26 INFO ZServer HTTP server started at Mon Jan  9 19:53:26
    2012
        Hostname: 0.0.0.0
        Port: 8080
    2012-01-09 19:53:29 WARNING ZODB.blob (13380) Blob dir
    /Users/aclark/Developer/test-plone/var/blobstorage/ has insecure mode setting
    2012-01-09 19:53:35 INFO PloneHotfix20110928 Hotfix installed.
    2012-01-09 19:53:35 INFO Zope Ready to handle requests

Open the following URL in your web browser:

 - http://127.0.0.1:8080

You should see:

.. image:: https://github.com/aclark4life/pythonpackages-docs/raw/master/ex5-plone-00.png
   :width: 294
   :height: 187

Happy times!

.. include:: disqus.html
