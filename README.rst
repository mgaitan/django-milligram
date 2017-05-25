Django-Milligram
=================



``django-miligram`` is a small django app to provide a base template
for your django project based on the open source `Milligram front-end framework <https://github.com/milligram/milligram>`_

django-milligram also works as a `pinax <https://github.com/pinax/pinax>`_ theme.


Getting Started
-----------------

Include ``django-milligram`` in your requirements file and include
``milligram`` in your ``INSTALLED APPS``.

Add ``django.core.context_processors.request`` to your ``TEMPLATE_CONTEXT_PROCESSORS``
to ensure the user selector and site name work correctly.

Make sure both template loaders and staticfiles finders includes
app directories.

Site name comes from Sites fixture.

Your ``site_base.html`` should extend ``milligram/base.html`` and should provide
``footer`` and ``nav`` blocks (the latter should just be a ul of li of a links).

Your pages should have blocks ``head_title`` and ``body`` and should extend
``site_base.html``.

The url name ``home`` should be defined as the homepage.


Examples
---------

- http://declaraciones.metrodelegados.com.ar


License
-------

It's released under the MIT license.


Contribute
-----------

Pull requests and ideas are welcome.

In order to foster a kind, inclusive, and harassment-free community, this project
project adheres to the `Python Community Code of Conduct <https://www.python.org/psf/codeofconduct/>`_.