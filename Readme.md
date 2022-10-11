# Learn Django 
![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=green)
## Create virtual env 
```bash
virtualen env || python -m virtualenv env
```

## Install requeriments 
```bash
pip install requeriments.txt 
```
# Create a project with django
```bash
django-admin startproject 'name your project' . 
# example
django-admin startproject myapp . 
```
## Run project 
```bash
python manage.py runserver || python manage.py runserver 3000
```
## Create an app
```bash
python manage.py startapp 'name your app'
# example
python manage.py startapp blog
```
## Create a views 
```bash
from django-http import HttpResponse
# Createa a view
def hello_view(request):
    return HttpResponse('Hello, world')
```
## Include your views in url path 
```bash
# import views
urlpatterns = [
    path('', views.hello_view)
]
```
## Interactue with db
```bash
python manage.py makemigrations
python manage.py migrate
```
## Create your models
```bash
from django.db import models
# create model
class Project(models.Mode):
    name = models.CharField(max_length=200)

class Model(models.Model):
    name =  models.CharField(max_length=200)
    description = TextField()
    project = models.ForeignKey(Project)
```
## Connect a database
```bash
# Examples
# Default
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',
    }
}

```
## Create data on databae
```bash
from myapp.models import Project, Task # Your models
projects = Project(name="Page Web with Django")
projects.save()
```
