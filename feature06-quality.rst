.. Note:: This is a work in progress

Package quality
---------------

`pythonpackages.com`_ evaluates the quality of a package based on criteria like description length
(i.e. too short?) and distribution formats uploaded (i.e. egg but no sdist?).
If your package meets the acceptable criteria you should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/feature06-quality-01.png

Otherwise you may see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/feature06-quality-00.png

This functionality is provided by a library called `pypi.trashfinder`_, which is
a pythonpackages.com-specific fork of `zopyx.trashfinder`_.

.. _`pythonpackages.com`: http://pythonpackages.com
.. _`pypi.trashfinder`: http://pythonpackages.com/package/pypi.trashfinder
.. _`zopyx.trashfinder`: http://pythonpackages.com/package/zopyx.trashfinder

.. include:: disqus.html
