django-app-template
========================

This is a template for creating a new reusable application for Django.
This uses the template feature added to the ``startapp`` command in Django 1.4. While
creating the app requires using Django 1.4 you can choose to support earlier versions
once it has been created.

To start a new app with this template::

    # Install Django
    pip install django>=1.4
    # Clone the repo
    git clone git://github.com/mlavin/django-app-template.git
    # Use the template
    django-admin.py startapp --template=django-app-template/template --extension=py,rst,in <app_name>


What Does This Give You
-----------------------------------

This template is indended to be used for a reusable application developed outside
of a Django project. Beyond the standard ``<app_name>/__init__.py``, ``<app_name>/models.py``,
``<app_name>/tests.py`` and ``<app_name>/views.py`` this template will create:

- README.rst - Some minor layout to get you started
- setup.py - A starting point for packaging your app
- MANIFEST.in - Includes your app templates and static resources
- AUTHORS - Add your name here
- LICENSE - Add a license here
- runtests.py - Simple helper for running the application tests
- tox.ini - Configured to run tests on Django 1.3/1.4/master on Python 2.6
- .gitignore/.hgignore - Just to save you a few key strokes


What To Do Next
-----------------------------------

This template gives you a good starting point for your application layout but there
are still some pieces of information to fill out:

- Write your app and tests
- Fill in the ``<app_name>/__init__.py`` doc string and ``__version__``
- Pick a license and add author names
- Write a more complete README
- Adjust the meta information in the ``setup.py``

You should also consider using `Sphinx <http://sphinx.pocoo.org/>`_ 
to create a more complete set of documentation. For than you can install Sphinx
and run the quickstart::

    # Install Sphinx
    pip install sphinx
    # Run the quickstart to create docs in docs/
    # Most other default answers should be fine
    sphinx-quickstart

When you are ready to upload your app to the Python Package Index (PyPi) you
can do that using the ``setup.py`` created with this template::

    # Register you package name and meta data (This is done once)
    python setup.py register
    # Create a release and upload it (This is done with every new version)
    python setup.py sdist upload


License Info
-----------------------------------

The template itself is available under the "Simplified" BSD license and can be
freely modified under the terms of that license. You can see the 
`full license text <https://github.com/mlavin/django-app-template/blob/master/LICENSE>`_  
in the Github repository for additional detail.

Applications created using this templates are not considered derivatives works.
Applications created using this template can be freely licensed under whatever
you as the author chooses. They may be either open or closed source.

If you are creating an open source application and need some direction on
available open source licenses for your new application, you can find information
on the `Open Source Initiative (OSI) <http://opensource.org/licenses/category>`_
website.


Contributing
-----------------------------------

Remember if these defaults don't work for you then you can always create a fork 
and update them to fit your own needs. If you have found a bug or have a suggestion
for an improvement which has broad appeal then please file a bug or submit
a pull request.
