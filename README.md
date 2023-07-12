# Ecommerce-App
Learning to create Django website from scratch

## Working in git bash environment
### Setup django virtual environment using:

python -m venv djangoenv (bash)

### To activate , VEnvironment 

source djangoenv/bin/activate (bash)

To confirm, its activate (environment name = djangoenv) before dir in cmd and also type pip freeze and it should return empty by default because we haven't installed any my default.

### Install Django Package
``` pip install django (bash) ```

### Install Django project
``` django-admin startproject obhEcommerce (if bash) ```

### Run Django project server
``` python manage.py runserver ```

### Migrate the default sqlite database (if default migrations are asked first)
``` python manage.py migrate ```

### For checking the DB Shell of sqlite using commandline
python manage.py dbshell 
Some Sqlite commands : 
 1. To list all SQLite tables  - ```. table . ```