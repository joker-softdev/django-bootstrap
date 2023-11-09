# django-bootstrap3

[![CI](https://github.com/zostera/django-bootstrap3/workflows/CI/badge.svg?branch=main)](https://github.com/zostera/django-bootstrap3/actions?workflow=CI)
[![Coverage Status](https://coveralls.io/repos/github/zostera/django-bootstrap3/badge.svg?branch=main)](https://coveralls.io/github/zostera/django-bootstrap3?branch=main)
[![Latest PyPI version](https://img.shields.io/pypi/v/django-bootstrap3.svg)](https://pypi.python.org/pypi/django-bootstrap3)

Bootstrap 3 for Django.

## Goal

The goal of this project is to seamlessly blend Django and Bootstrap 3.

- Want to use Bootstrap 4 in Django? See https://github.com/zostera/django-bootstrap4.
- Want to use Bootstrap 5 in Django? See https://github.com/zostera/django-bootstrap5.

## Requirements

This package requires a combination of Python and Django that is currently supported.

See "Supported Versions" on https://www.djangoproject.com/download/.

## Documentation

The full documentation is at https://django-bootstrap3.readthedocs.io/

## Installation

1. Install using pip:

    ```shell script
    pip install django-bootstrap3
    ```

   Alternatively, you can install download or clone this repo and call ``pip install -e .``.

2. Add to `INSTALLED_APPS` in your `settings.py`:

   ```python
   INSTALLED_APPS = (
       # ...
       "bootstrap3",
       # ...
   )
   ````

3. In your templates, load the `bootstrap3` library and use the `bootstrap_*` tags:

## Example template

```djangotemplate
{% load bootstrap3 %}

{# Display a form #}

<form action="/url/to/submit/" method="post" class="form">
    {% csrf_token %}
    {% bootstrap_form form %}
    {% buttons %}
        <button type="submit" class="btn btn-primary">Submit</button>
    {% endbuttons %}
</form>
```

Example app
-----------

An example app is provided in `example`. You can run it with `make example`.


Bugs and suggestions
--------------------

If you have found a bug or if you have a request for additional functionality, please use the issue tracker on GitHub.

https://github.com/zostera/django-bootstrap3/issues


License
-------

You can use this under BSD-3-Clause. See [LICENSE](LICENSE) file for details.


Author
------

Developed and maintained by [Zostera](https://zostera.nl).

Original author: [Dylan Verheul](https://github.com/dyve).

Thanks to everybody that has contributed pull requests, ideas, issues, comments and kind words.

Please see [AUTHORS](AUTHORS) for a list of contributors.
