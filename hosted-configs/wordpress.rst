.. Note:: `View config on GitHub`_
  :class: alert alert-info

Wordpress
=========

The award-winning, PHP-based blogging software, Wordpress. You want to download and install Wordpress and keep it up to date with only a few commands::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = https://raw.github.com/pythonpackages/buildout-wordpress/master/3.4.x

Then run::

    $ bin/buildout

This will install the Wordpress files in ``parts/wordress`` at which point you can
configure your PHP-powered Apache to use them.

.. include:: ../disqus.html

.. _`View config on GitHub`: https://github.com/pythonpackages/buildout-wordpress/blob/master/3.4.x
