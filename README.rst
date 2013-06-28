django-simple-history
=====================

.. image:: https://secure.travis-ci.org/treyhunner/django-simple-history.png?branch=master
   :target: http://travis-ci.org/treyhunner/django-simple-history
.. image:: https://coveralls.io/repos/treyhunner/django-simple-history/badge.png?branch=master
   :target: https://coveralls.io/r/treyhunner/django-simple-history
.. image:: https://pypip.in/v/django-simple-history/badge.png
   :target: https://crate.io/packages/django-simple-history
.. image:: https://pypip.in/d/django-simple-history/badge.png
   :target: https://crate.io/packages/django-simple-history

django-simple-history stores Django model state on every create/update/delete.

This app requires Django 1.3.7 or greater and Python 2.6 or greater.

This fork adds automatic setting of the history_user field but requires you to
change your settings.py file.
Append the following line to your MIDDLEWARE_CLASSES:
'simple_history.middleware.CurrentUserMiddleware',

e.g.
MIDDLEWARE_CLASSES = (
  ...
  'simple_history.middleware.CurrentUserMiddleware',
  ...
)


Getting Help
------------

Documentation is available at https://django-simple-history.readthedocs.org/

Issue tracker is at https://github.com/treyhunner/django-simple-history/issues

Pull requests are welcome.  Read the CONTRIBUTING file for tips on
submitting a pull request.

.. _PyPI: https://pypi.python.org/pypi/django-email-log/
