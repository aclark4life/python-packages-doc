.. Note:: `View config on GitHub`_
  :class: alert alert-info

Django
======

In this example, we configure a "hello world" application for your Django-ing pleasure::

    $ virtualenv-2.7 .
    $ bin/pip install zc.buildout
    $ bin/buildout init

Then edit the contents of **buildout.cfg** to contain *only*::

    [buildout]
    extends = http://pythonpackages.com/buildout/django/1.4.x

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

And open the following URL in your web browser:

 - http://127.0.0.1:8000/admin/

You should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/hosted-configs/django1.png
   :class: thumbnail


Everywhere else you should see:

.. image:: https://github.com/pythonpackages/pythonpackages-docs/raw/master/hosted-configs/django2.png
   :class: thumbnail

.. include:: ../disqus.html

.. _`View config on GitHub`: https://github.com/pythonpackages/buildout-django/blob/master/1.4.x
