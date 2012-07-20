.. include:: note-about-build-section.rst

Example #9 - funnelweb
======================

Easily import content into the award-winning, Python-based, Plone CMS.


Import content to ``Plone`` with funnelweb
------------------------------------------

You want to import your non-Plone website content into ``Plone``::

    $ virtualenv-2.6 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://pythonpackages.com/buildout/plone/4.1.x
    parts += funnelweb

    [funnelweb]
    recipe = funnelweb
    

Then run::

    $ bin/buildout

Followed by::

    $ bin/plone start

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

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/ex5-plone-00.png
   :width: 294
   :height: 187

Now create a Plone site and run::

    $ bin/funnelweb --crawler:url=http://example.com --ploneupload:target=http://admin:admin@localhost:8080/Plone

You should see in the terminal::

    INFO:titleguess(pathsorter):2 folders added. 0 defaultpages set, 3 items sorted
    WARNING:urltidy:22 broken internal links. Content maybe missing. Debug to see
    details.
    INFO:addfolders(pathsorter):0 folders added. 0 defaultpages set, 3 items sorted
    INFO:ploneupload(pathsorter):0 folders added. 0 defaultpages set, 3 items
    sorted
    INFO:plonepublish: performing transition 'publish'
    INFO:plonepublish:domains performing transition 'publish'
    INFO:ploneupload:domains/example Created with type=Document
    INFO:ploneupdate:domains/example set fields=['text', 'ContentType']
    INFO:plonepublish:domains/example performing transition 'publish'

And in Plone:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/ex9-funnelweb-00.png
   :width: 345
   :height: 342.5

Happy times!

.. include:: disqus.html
