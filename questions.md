# Code Questions


## 2022-03-26

- Why does registration-redux direct me to '/accounts/login/habits' instead of just 'habits/'?

## 2022-03-25

- Tracing the file paths through the Django source code, `AppConfig` in django.apps is really a Class in the file `config.py` found by the path from the root of : `Django/django/apps/config.py`

- When we write `user = request.user` in our view.py files, where does that `user` attribute come from?  