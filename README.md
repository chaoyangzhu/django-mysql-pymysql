django-mysql-pymysql
====================

This is a Django database backend for MySQL, using the PyMySQL database adapter. It is intended to be a drop-in replacement for the built-in MySQLdb backend, and leverages quite a bit of its code.

This fork is updated to work for Django 1.5.2. Tested under Python 3.3.2.


Requirements
------------

* Django 1.5.2
* PyMySQL (patches here: https://github.com/clelland/PyMySQL)

Installation
------------

1. Clone and install into your site-packages directory:

        $ git clone https://github.com/clelland/django-mysql-pymysql
        $ cd django-mysql-pymysql
        $ python setup.py install

2. Edit your settings file:

        DATABASES = {
            'default': {
                'ENGINE': 'mysql_pymysql',
                'HOST': ...,
                'USER': ...,
                'PASSWORD': ...,
            }
        }


3. You're done.
