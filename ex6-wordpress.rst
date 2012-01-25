.. include:: note-about-build-section.rst

Example #6
==========

The award-winning, PHP-based blogging software, Wordpress.

``Wordpress`` installation
--------------------------

You want to download and install Wordpress and keep it up to date with only a
few commands:: 

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://build.pythonpackages.com/buildout/wordpress/latest

Then run::

    $ bin/buildout

This will install the Wordpress files in ``parts/wordress`` at which point you can
configure your PHP-powered Apache to use them.

Happy times!

.. include:: disqus.html
