# django-social-authentication (github login)

A Django Social Authentication via django-allauth

## Features

* Django 2.0 and Python 3.6
* [django-allauth](https://github.com/pennersr/django-allauth) for easy social auth
* [Pipenv](https://github.com/pypa/pipenv) for virtualenvs

## First-time setup

1.  Make sure Python 3.6x and Pipenv are already installed. [See here for help](https://djangoforbeginners.com/initial-setup/).

2.  Clone the repo and configure the virtual environment:

```
$ git clone https://github.com/omjigupta/django-social-authentication.git
$ cd django-social-authentication
$ pipenv install
$ pipenv shell
```

3.  Set up the initial migration for our custom user models in users and build the database.

```
(django-social-authentication) $ python manage.py makemigrations users
(django-social-authentication) $ python manage.py migrate
(django-social-authentication) $ python manage.py createsuperuser
(django-social-authentication) $ python manage.py runserver
```

4.  Endpoints

Login to github

* login - http://127.0.0.1:8000/
