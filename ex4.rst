.. include:: section-note.rst

Example #4
==========

Many developers install ``Django`` with::

    $ pip install Django

But after it's installed, additional setup is required (i.e. editing settings.py etc.) If you
are a beginner, you may want more done for you automatically (a la "installers").

``Django`` installation
-----------------------

You want to take ``Django`` for a spin, but you don't know much about it or
Python::

    $ virtualenv .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Then you edit the contents of buildout.cfg to contain *only*::

    [buildout]
    extends = http://build.pythonpackages.com/buildout/django/latest

Then run::

    $ bin/buildout

Followed by::

    $ bin/django syncdb

At which point you should see::

    Creating tables ...
    Creating table auth_permission
    Creating table auth_group_permissions
    Creating table auth_group
    Creating table auth_user_user_permissions
    Creating table auth_user_groups
    Creating table auth_user
    Creating table auth_message
    Creating table django_content_type
    Creating table django_session
    Creating table django_site
    Creating table django_admin_log

Followed by a prompt for your username and new password::

    You just installed Django's auth system, which means you don't have any
    superusers defined.
    Would you like to create one now? (yes/no): yes
    Username (Leave blank to use 'aclark'): admin
    E-mail address: aclark@aclark.net
    Password: 
    Password (again): 
    Superuser created successfully.
    Installing custom SQL ...
    Installing indexes ...
    No fixtures found.

After which you can run::

    $ bin/django runserver

Open the following URL in your web browser:

 - http://127.0.0.1:8000/admin/

And you should see:

.. image:: https://github.com/aclark4life/pythonpackages-docs/raw/master/django.png

Happy times!
