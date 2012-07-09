.. include:: note-about-build-section.rst

Example #7 - PloneGetPaid
=========================

E-commerce platform for Plone: getpaid.

``getpaid`` for Plone
---------------------

You want to try ``getpaid`` for Plone::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://pythonpackages.com/buildout/plone-getpaid/4.2.x

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

Click on "Create a new plone site" and should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/ex7-getpaid-00.png
   :width: 365.5
   :height: 353

Happy times!

.. include:: disqus.html
