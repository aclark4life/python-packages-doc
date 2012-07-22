.. include:: note-about-build-section.rst

Example #6 - Wordpress
======================

The award-winning, PHP-based blogging software, Wordpress. You want to download and install Wordpress and keep it up to date with only a few commands::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://pythonpackages.com/buildout/wordpress/3.3.x

Then run::

    $ bin/buildout

This will install the Wordpress files in ``parts/wordress`` at which point you can
configure your PHP-powered Apache to use them.

.. include:: disqus.html
