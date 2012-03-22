.. include:: note-about-build-section.rst

Advanced
========

This section contains information about an advanced feature of
pythonpackages.com: hosted configuration files.

Buildout/easy_install vs. virtualenv/pip
----------------------------------------

What do most Python programmers do for a living? They build things like:
software, services, systems and so on.

How can we make building things (with Python) easier for everyone involved? By providing
clear and concise documentation.

Further, let us not debate about which tool is best. We have lots of **tools** in
the Python world. What we are missing is **clarity**. Rather than force people to use
a particular tool without explaining why, let us *better* explain what tools
are available and let folks decide for themselves which ones they would like to use. In the
case of ``zc.buildout`` and ``pip``, we can provide sample configuration files to
demonstrate their use.

Hosted configuration files
--------------------------

In addition to its core features, ``pythonpackages.com`` provides a set of shared,
extendable configuration files for building Python-based and other software.
Please continue reading to see examples.

Contents:

.. toctree::
   :maxdepth: 1
   :glob:

   ex1-jenkins
   ex2-apache
   ex3-bluebream
   ex4-django
   ex5-plone
   ex6-wordpress
   ex7-getpaid
   ex8-diazo
   ex9-funnelweb
   ex10-plone

.. include:: disqus.html
