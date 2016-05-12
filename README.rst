======================
Bootstrap 4 for Django
======================

Write Django as usual, and let ``django-bootstrap4`` make template output into Bootstrap 4 code.


.. image:: https://img.shields.io/travis/GabrielUlici/django-bootstrap4/master.svg
    :target: https://travis-ci.org/GabrielUlici/django-bootstrap4

.. image:: https://img.shields.io/coveralls/GabrielUlici/django-bootstrap4/master.svg
  :target: https://coveralls.io/r/GabrielUlici/django-bootstrap4?branch=master


Requirements
------------

- Python 2.7, 3.2, 3.3, 3.4, or 3.5
- Django >= 1.8


Installation
------------

1. Install using pip:

   ``pip install django-bootstrap4``

   Alternatively, you can install download or clone this repo and call ``pip install -e .``.

2. Add to INSTALLED_APPS in your ``settings.py``:

   ``'bootstrap4',``

3. In your templates, load the ``bootstrap4`` library and use the ``bootstrap_*`` tags:

This app will soon require Django 1.8+, python 2.7+. Thanks for understanding.


Example template
----------------

   .. code:: Django

    {% load bootstrap4 %}

    {# Display a form #}

    <form action="/url/to/submit/" method="post" class="form">
        {% csrf_token %}
        {% bootstrap_form form %}
        {% buttons %}
            <button type="submit" class="btn btn-primary">
                {% bootstrap_icon "star" %} Submit
            </button>
        {% endbuttons %}
    </form>


.. Documentation
.. -------------

.. The full documentation is at http://django-bootstrap4.readthedocs.org/.


Bugs and suggestions
--------------------

If you have found a bug or if you have a request for additional functionality, please use the issue tracker on GitHub.

https://github.com/GabrielUlici/django-bootstrap4/issues


License
-------

You can use this under Apache 2.0. See `LICENSE
<LICENSE>`_ file for details.


Author
------

.. Developed and maintained by `Zostera <https://zostera.nl/>`_.

Original author : `Dylan Verheul <https://github.com/dyve>`_.

Development lead: `Gabriel Ulici <https://github.com/GabrielUlici>`_.

Thanks to everybody that has contributed pull requests, ideas, issues, comments and kind words.

Please see AUTHORS.rst for a list of contributors.
