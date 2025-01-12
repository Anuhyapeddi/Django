# Django

* Django is python's framework used to build website.
* Django Rest Framework is a toolkit used to build api's.
* company's like instagram, pinterest and spotify uses django rest framework.
* it generally used because it is fast, have many components, gives security and scalability.

Files in Django Project:

* _init_.py - Tells python treat this directory as a python package.
* asgi.py  and wsgi.py - These are special configuration files that we don't need to deal with, but these files helps django to communicate with the server
* settings.py - used to install different django application, install pulgins, chaging middleware, chaging database engine, and also deploy in the server using secret_key
* urls.py - used to configure different urls routes that can direct to different django applications.
* manage.py - act like a command line tool, it allows us to run special commands like make database migrations and run python server.
* admin.py - register database models to view them on admin panel.
* models.py - where we write our database models.
* tests.py -  where we write some automated testcases.
* views.py - where we can create and access out websites request.

Creating new app and ruuning in django project:

* To create a new app - python3 manage.py startapp app_name
* To run the django application - python3 manage.py runserver
