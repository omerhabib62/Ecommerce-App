# Ecommerce-App
Learning to create Django website from scratch. The app is created is Django app with MySQL database in gitpod.

Learning Sources: 
1. [Ecommerce Tutorial](https://www.youtube.com/watch?v=YZvRrldjf1Y&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ&start_radio=1&ab_channel=freeCodeCamp.org)
2. [Full Stack Development course in the Cloud - Svelte, Postgres, Vercel, Gitpod - for learning working on gitpod](https://www.youtube.com/watch?v=OUzaUJ3gEug&t=10s&ab_channel=freeCodeCamp.org)
3. [Django Docs](https://docs.djangoproject.com/)

## Notes:
### What’s the difference between a project and an app? 
1. An app is a web application that does something – e.g., a blog system, a database of public records or a small poll app. A project is a collection of configurations and apps for a particular website. A project can contain multiple apps. An app can be in multiple projects.
2. i. Project in cmd = startproject
   ii. App in cmd = startapp
3. URLS are not there , need to create a file for URLs in an app and then add to the project/urls.py
4. The <ins>path()</ins> function is passed four arguments, two required: route and view, and two optional: kwargs, and name. At this point, it’s worth reviewing what these arguments are for.

### Favourite Extensions
1. Python - by Microsoft
2. Intellicode - by Microsoft
3. Django - by Baptiste Darthenay
4. Python Environment Manager - by Don Jayamanne

## Working in git bash environment
### Setup django virtual environment using:

python -m venv djangoenv (bash)

### To activate, VEnvironment 

```  source djangoenv/bin/activate (bash)  ```
``` djangoenv\Scripts\activate (cmd) ``` 

To confirm, activate (environment name = djangoenv) before dir in cmd and also type pip freeze and it should return empty by default because we haven't installed any my default.

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
``` python manage.py dumpdata > ecommercesqlite.json ```

 #### 2. Create Database using MySQLClient (in gitpod)

 ### Creating a project in django Project(Django project  = django-admin startproject <project-name>)
 ``` python manage.py startapp polls ```
 
