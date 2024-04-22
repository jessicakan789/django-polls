# Django Poll App
The [Django Tutorial](https://docs.djangoproject.com/en/5.0/intro/tutorial01/) was followed to create an app that allows the user to answer a poll question.

## How to install
```
python -m pip install Django

git clone https://github.com/jessicakan789/django-polls
```

### OPTIONAL: install app as package
```
python -m pip install --user dist/django-polls-0.1.tar.gz
```

## How to use
```
cd django-polls

python manage.py runserver 
```

Navigate to http://127.0.0.1:8000/ in a browser

Click on "What's up?"

Then answer the poll question and use "Vote again" to vote again.

## Updating the database
```
python manage.py migrate

python manage.py makemigrations <app_label>

python manage.py sqlmigrate <app_label> <migration_number>

python manage.py migrate
```

## Admin notes
```
python manage.py createsuperuser  # To create admin account
```

Navigate to http://127.0.0.1:8000/admin in a browser

## Project notes
manage.py: A command-line utility that lets you interact with this Django project in various ways. You can read all the details about manage.py in django-admin and manage.py.

The inner mysite/ directory is the actual Python package for your project. Its name is the Python package name you’ll need to use to import anything inside it (e.g. mysite.urls).

mysite/__init__.py: An empty file that tells Python that this directory should be considered a Python package. If you’re a Python beginner, read more about packages in the official Python docs.

mysite/settings.py: Settings/configuration for this Django project. Django settings will tell you all about how settings work.

mysite/urls.py: The URL declarations for this Django project; a “table of contents” of your Django-powered site. You can read more about URLs in URL dispatcher.

mysite/asgi.py: An entry-point for ASGI-compatible web servers to serve your project. See How to deploy with ASGI for more details.

mysite/wsgi.py: An entry-point for WSGI-compatible web servers to serve your project. See How to deploy with WSGI for more details.

# App notes
django_polls/views.py: A view is a function or method that takes http requests as arguments, imports the relevant model(s), and finds out what data to send to the template, and returns the final result.

django_polls/models.py: The model provides data from the database.

django_polls/templates: A template is a file where you describe how the result should be represented.

django_polls/urls.py: Django also provides a way to navigate around the different pages in a website.

django_polls/static: Aside from the HTML generated by the server, web applications generally need to serve additional files — such as images, JavaScript, or CSS — necessary to render the complete web page. In Django, we refer to these files as “static files”.

REFERENCE: [W3 Schools](https://www.w3schools.com/django/index.php)

# Tree
```
.
├── db.sqlite3
├── django_polls
│   ├── admin.py
│   ├── apps.py
│   ├── dist
│   │   └── django-polls-0.1.tar.gz
│   ├── django_polls.egg-info
│   │   ├── dependency_links.txt
│   │   ├── PKG-INFO
│   │   ├── requires.txt
│   │   ├── SOURCES.txt
│   │   └── top_level.txt
│   ├── docs
│   ├── __init__.py
│   ├── LICENCE
│   ├── MANIFEST.in
│   ├── migrations
│   │   ├── 0001_initial.py
│   │   ├── __init__.py
│   │   └── __pycache__
│   │       ├── 0001_initial.cpython-310.pyc
│   │       └── __init__.cpython-310.pyc
│   ├── models.py
│   ├── __pycache__
│   │   ├── admin.cpython-310.pyc
│   │   ├── apps.cpython-310.pyc
│   │   ├── __init__.cpython-310.pyc
│   │   ├── models.cpython-310.pyc
│   │   ├── tests.cpython-310.pyc
│   │   ├── urls.cpython-310.pyc
│   │   └── views.cpython-310.pyc
│   ├── pyproject.toml
│   ├── README.rst
│   ├── setup.cfg
│   ├── setup.py
│   ├── static
│   │   └── polls
│   │       ├── images
│   │       │   └── background.png
│   │       └── style.css
│   ├── templates
│   │   ├── admin
│   │   ├── base.html
│   │   ├── base_site.html
│   │   └── polls
│   │       ├── detail.html
│   │       ├── index.html
│   │       └── results.html
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── manage.py
├── mysite
│   ├── asgi.py
│   ├── __init__.py
│   ├── __pycache__
│   │   ├── __init__.cpython-310.pyc
│   │   ├── settings.cpython-310.pyc
│   │   ├── urls.cpython-310.pyc
│   │   ├── views.cpython-310.pyc
│   │   └── wsgi.cpython-310.pyc
│   ├── settings.py
│   ├── urls.py
│   ├── views.py
│   └── wsgi.py
└── README.md
```
