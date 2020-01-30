=============
ckanext-datagovrov2_theme
=============



------------
Requirements
------------

Built for https://github.com/john21ro/ckan version.


------------
Installation
------------

.. Add any additional install steps to the list below.
   For example installing any non-Python dependencies or adding any required
   config settings.

To install ckanext-datagovrov2_theme:

1. Activate your CKAN virtual environment, for example::

     . /usr/lib/ckan/default/bin/activate

2. Clone and install the ckanext-datagovrov2_theme Python package into your virtual environment::

     python setup.py develop

3. Add ``datagovrov2_theme`` to the ``ckan.plugins`` setting in your CKAN
   config file (by default the config file is located at
   ``/etc/ckan/default/production.ini``).

4. Restart CKAN. For example if you've deployed CKAN with Apache on Ubuntu::

     sudo service apache2 reload


---------------
Config Settings
---------------

```
datagovrov2_theme.custom_resource_download_url = http://data.gov.ro
datagovrov2_theme.google_analytics_token_path = /etc/ckan/default/google-analytics-secrets.json
```

-----------------
Running the Tests
-----------------

To run the tests, do::

    nosetests --nologcapture --with-pylons=test.ini
