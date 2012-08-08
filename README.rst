django-app-template
========================

This is a template for creating a new reusable application for Django. This uses
the template feature added to the ``startapp`` command in Django 1.4. While
creating the app requires using Django 1.4 you can choose to support earlier versions
once it has been created.

To start a new app with this template::

    # Install Django
    pip install django>=1.4
    # Clone the repo
    git clone git://github.com/mlavin/django-app-template.git
    # Use the template
    django-admin.py startapp --template=django-app-template/template --extension=py,rst,in <app_name>


What Does This Give You?
-----------------------------------

Beyond the standard ``<app_name>/__init__.py``, ``<app_name>/models.py``,
``<app_name>/tests.py`` and ``<app_name>/views.py`` this template will create

 * README.rst - Some minor layout to get you started
 * setup.py - A starting point for packaging your app
 * MANIFEST.in - Includes your app templates and static resources
 * AUTHORS - Add your name here
 * LICENSE - Add a license here
 * runtests.py - Simple helper for running the application tests
 * tox.ini - Configured to run tests on Django 1.3/1.4 on Python 2.6
 * .gitignore/.hgignore - Just to save you a few key strokes

