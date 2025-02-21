# Django

* Django is python's framework used to build website.
* Django Rest Framework is a toolkit used to build api's.
* company's like instagram, pinterest and spotify uses django rest framework.
* it generally used because it is fast, have many components, gives security and scalability.

How to create a new project

* Go to the directory where you want to create a project
* python3 -m venv venv - to create a virtual environment (Before this I have create another project of django, so to avoid configuratuion issue I have create a virual env)
* source venv/bin/activate - to activate the virtual environment
* pip3 install django - install django (here django web framework)
* pip3 install django djangorestframework - install the django rest framework (used to create rest api's)

Creating new app and runing in django project:

* To create a new app - python3 manage.py startapp app_name
* To make migration - python3 manage.py makemigrations
* python3 manage.py migrate
* To run the django application - python3 manage.py runserver

Files in Django Project:

* _init_.py - Tells python treat this directory as a python package.
* asgi.py  and wsgi.py - These are special configuration files that we don't need to deal with, but these files helps django to communicate with the server
* settings.py - used to install different django application, install pulgins, changing middleware, changing database engine, and also deploy in the server using secret_key
* urls.py - used to configure different urls routes that can direct to different django applications.
* manage.py - act like a command line tool, it allows us to run special commands like make database migrations and run python server.
* admin.py - register database models to view them on admin panel.
* models.py - where we write our database models.
* serializer.py - here we convert our model to JSON formate which we can access by api.
* tests.py -  where we write some automated testcases.
* views.py - where we can create and access out websites request.

Django Template Language (NOTE: Avoid this if you are working with backend)

* we can send HTML scripts in response
```python
  def home(request):
      return HttpResponse('<h1>Hello World</h1>')
```
* what if we have large file of HTML, and HTML files are static files. To make it dynamic we have to use Django Template Language.
* create a template folder and create a html file in it.
* Now, call the html file
```python
  def home(request):
      return render(request, 'file_name.html')
```

Flow

user -> django -> url -> view -> template and model -> database











