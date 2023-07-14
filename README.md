# Ecommerce-App
Learning to create Django website from scratch. The app is created is Django app with MySQL database in gitpod.

Learning Sources: 
1. [Ecommerce Tutorial](https://www.youtube.com/watch?v=YZvRrldjf1Y&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ&start_radio=1&ab_channel=freeCodeCamp.org)
2. [Full Stack Development course in the Cloud - Svelte, Postgres, Vercel, Gitpod - for learning working on gitpod](https://www.youtube.com/watch?v=OUzaUJ3gEug&t=10s&ab_channel=freeCodeCamp.org)
3. [Django Docs](https://docs.djangoproject.com/)


## Working in git bash environment
### Setup django virtual environment using:

python -m venv djangoenv (bash)

### To activate , VEnvironment 

```  source djangoenv/bin/activate (bash)  ```
``` djangoenv\Scripts\activate (cmd) ``` 

To confirm, its activate (environment name = djangoenv) before dir in cmd and also type pip freeze and it should return empty by default because we haven't installed any my default.

### Install Django Package
``` pip install django (bash) ```

### Install Django project
``` django-admin startproject obhEcommerce (bash) ```

### Run Django project server
``` python manage.py runserver ```

### Migrate the default sqlite database (if default migrations are asked first)
``` python manage.py migrate ```

### For checking the DB Shell of sqlite using commandline
python manage.py dbshell 
Some Sqlite commands : 
 1. To list all SQLite tables  - ```. table . ```
 
 ### Migrating DB from SQLite to MySQL Database 
 I am going to change SQLite using cmdline.
 

 #### 1. Export Database in json format
 python manage.py dumpdata > ecommercesqlite.json

 #### 2. Create Database using MySQLClient (in gitpod)
