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


