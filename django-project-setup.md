# Django Project Setup

1. Create local directory
2. Install django with pipenv, as well as Pipfile and Piplock:
habbit
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
$ django-admin startapp users 
```


## Custom User
4. Add a custom user app as good practice for creating a custom user class
```sh
$ django-admin startapp users 
```

Once this is created, go to to models.py within the app directory that was just created and add:

```py
from django.contrib.auth.models import AbstractUser

class CustomUser(AbstractUser):
    pass
    def __str__(self):
        return self.username
```

- here is a great reference / tutorial for setting up a [Custom User Model](https://learndjango.com/tutorials/django-custom-user-model). **NOTE:** remember to do this before making migrations to the database!!

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

## Extensions 

---
  
### django-registration-redux
[Documentation](https://django-registration-redux.readthedocs.io/en/latest/quickstart.html)

```sh
$ pipenv install django-registration-redux
```
**Settings**
- Install django.contrib.auth and django.contrib.sites to the project 

<hr>

### django-environ
[Documentation](https://django-environ.readthedocs.io/en/latest/)

```sh
$ pipenv install django-environ
```
**Settings**
- After install create a `.env` file in project root directory with the following sample example from our 'Flashcards' app:


## 
 ```sh 
SECRET_KEY='django-insecure-6^g(edzu^8$*4zqud36mxge%d22*k)8y*f^5zcfda8(n4=hkv^'
DEBUG=True
DATABASE_URL=postgres://habbit-tracker:@127.0.0.1:5432/habbit-tracker
 ```

- take the secret key from settings.py and use the documentation to modify settings.py accordingly. 




