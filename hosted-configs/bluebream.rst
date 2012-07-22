.. include:: note-about-build-section.rst

Bluebream
=========

Formerly "Zope 3 application server". You have heard that the Zope 3 application server, the successor to the world famous
``Zope2`` application server is now called ``Bluebream`` and you want to try it out::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Then edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://pythonpackages.com/buildout/bluebream/1.0

Then run::

    $ bin/buildout

Followed by::

    $ bin/supervisord -e debug -n

At which point you should see::

    2011-12-22 15:27:30,238 INFO success: bluebream entered RUNNING state, process
    has stayed up for > than 1 seconds (startsecs)
    2011-12-22 15:27:31,037 DEBG 'bluebream' stdout output:
    ------
    2011-12-22T15:27:31 WARNING root Developer mode is enabled: this is a security
    risk and should NOT be enabled on production servers. Developer mode can
    usually be turned off by setting the `devmode` option to `off` or by removing
    it from the instance configuration file completely.

    2011-12-22 15:27:32,792 DEBG 'bluebream' stdout output:
    ------
    2011-12-22T15:27:32 INFO ZODB.blob (31588) Blob directory var/blobstorage does
    not exist. Selected `bushy` layout. 

    2011-12-22 15:27:32,792 DEBG 'bluebream' stdout output:
    ------
    2011-12-22T15:27:32 INFO ZODB.blob (31588) Blob directory
    '/Users/aclark/Developer/test-bluebream/var/blobstorage/' does not exist.
    Created new directory.

    2011-12-22 15:27:32,792 DEBG 'bluebream' stdout output:
    ------
    2011-12-22T15:27:32 INFO ZODB.blob (31588) Blob temporary directory
    'var/blobstorage/tmp' does not exist. Created new directory.

Open the following URL in your web browser:

 - http://127.0.0.1:8080

And you should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/hosted-configs/bluebream1.png
   :width: 248
   :height: 144
   :class: thumbnail

.. include:: ../disqus.html
