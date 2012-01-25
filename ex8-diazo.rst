.. include:: note-about-build-section.rst

Example #8
==========

How to theme the award-winning, Python-based, Plone CMS.

``Diazo`` theming in Plone
--------------------------

You want to take the new ``Diazo`` theming engine for ``Plone`` for a spin.

Part I: Setting up Plone
~~~~~~~~~~~~~~~~~~~~~~~~

Follow these steps::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://build.pythonpackages.com/buildout/plone/latest

    [plone]
    resources = ${buildout:directory}/resources

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

.. image:: https://github.com/aclark4life/pythonpackages-docs/raw/master/plone.png

Create a new Plone site then move on to Part II.

Part II: Setting up a new theme
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Now CTRL-C Plone and do the following::

    $ mkdir -p resources/theme/my.theme
    $ touch resources/theme/my.theme/index.html
    $ touch resources/theme/my.theme/rules.xml

Now restart Plone. Click on `Site Setup -> Diazo theme -> Advanced settings`. Make your
fields look like this:

.. image:: https://github.com/aclark4life/pythonpackages-docs/raw/master/diazo.png

Save the form. Select `Basic settings`. Select `Other` and enable your theme:

.. image:: https://github.com/aclark4life/pythonpackages-docs/raw/master/diazo2.png

Return to the site root. You should see… no change! One more step. Edit
index.html to contain::

    <div id="content"><h1>You can haz it!</h1></div>

And rules.xml to contain::

    <rules
        xmlns="http://namespaces.plone.org/diazo"
        xmlns:css="http://namespaces.plone.org/diazo/css"
        xmlns:xsl="http://www.w3.org/1999/XSL/Transform">

        <theme href="index.html" />

        <append css:theme="#content" css:content="#content"/>

    </rules>

Open the following URL in your web browser:

 - http://localhost:8080/Plone

.. Note:: Note the change from 127.0.0.1 to localhost

You should see:

.. image:: https://github.com/aclark4life/pythonpackages-docs/raw/master/diazo3.png


Conclusion
~~~~~~~~~~

Happy times! This, along with http://diazo.org, should be all any web-savvy person (who does not know any
Plone) needs to get started theming Plone.

.. include:: disqus.html
