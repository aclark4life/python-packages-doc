.. include:: section-note.rst

Example #3
==========

Remember Zope? Well, it's still around (and doing fine, thank you). It took
about 10 years to sort out the "rewrite" of the original, very famous,
"application server" package. The result is literally hundreds of Zope-related
Python packages grouped together under the project name "Zope Toolkit".

Never heard of Zope? Well, it is a very well known rapid web
application development environment, made very popular
in the early 2000s by its ability to enable web development **through-the-web**
(a technique that has since fallen out of favor, replaced by file system
development and software version control). You may think of it as the 
"Django/Pyramid/Flask/bottle/web2py" of its day. In fact, it was the very first
Python web framework.

Now-a-days, that application server is still in use, and maintained under the
package name "Zope2" (http://pythonpackages.com/info/zope2). Other Zope-related
technologies are in active development under various and sundry names. One such
project/package is called ``Bluebream``.

``Bluebream`` installation
--------------------------

You have heard that the Zope 3 application server, the successor to the world famous
``Zope2`` application server is now called ``Bluebream`` and you want to try it
out::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Then edit the contents of buildout.cfg to contain *only*::

    [buildout]
    extends = http://build.pythonpackages.com/buildout/bluebream/latest

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

.. image:: https://github.com/aclark4life/pythonpackages-docs/raw/master/bluebream.png

Happy times!
