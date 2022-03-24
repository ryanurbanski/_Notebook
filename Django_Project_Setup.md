# Django Project Setup
1. Create local directory
2. Install django with pipenv, as well as Pipfile and Piplock:

```sh
$ pipenv install django
```

3. Start virtual environment:
```sh
$ pipenv shell
```

4. Start project and name the root folder 'config' in the current directory:
```sh
$ django-admin startproject config .
```

5. Migrate to SQLite local db for development:
- (pmm) is set as this alias
```sh
$ python manage.py migrate
$ pmm
```

6. Start first app
```sh
$ pm startapp <appName>
```

7. Run Server
```sh
$ prs
$ prs 8001
$ python manage.py runserver
$ python manage.py runserver 8001
```
- Note: adding a port on the end will specify where to run the server
- prs is the alias I set up to run the server

8. Create superuser
```sh
$ pm createsuperuser
$ python manage.py createsuperuser
```

<br>

## Install Packages

---
  
### django-registration-redux
[Documentation](https://django-registration-redux.readthedocs.io/en/latest/quickstart.html)

```sh
$ pipenv install django-registration-redux
```
**Settings**
- Install django.contrib.auth and django.contrib.sites to the project 








