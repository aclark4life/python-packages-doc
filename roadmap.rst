.. roadmap:

The roadmap for the beta period (Q3 2012) is as follows:

Add AJAX and asynchronous task queues
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Currently all tasks are executed synchronously. This is a problem for large packages or packages with a lot of dependencies and/or tests because web requests will timeout before the tasks complete. It's also bad from a user interface perspective, so AJAX views and asynchronous tasks queues will be added to address these problems.

Windows workers
~~~~~~~~~~~~~~~

Currently pythonpackages.com is only capable of building source distributions (sdist) on Ubuntu Linux (via Heroku).

