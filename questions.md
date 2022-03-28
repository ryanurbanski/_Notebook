# Code Questions


## 2022-03-28

- Learning question: I want to create a radio for a boolean value in my form.
- I open django source code and search for the Class I want.
- class ModelForm is in models.py inside the django/forms directory.. so when we write from django import forms do we get access then to all 'modules' and classes within them? 
- class ModelForm inherits from BaseModelForm, so I go to that source

- 

## 2022-03-26

- Why does registration-redux direct me to '/accounts/login/habits' instead of just 'habits/'?

## 2022-03-25

- Tracing the file paths through the Django source code, `AppConfig` in django.apps is really a Class in the file `config.py` found by the path from the root of : `Django/django/apps/config.py`

- When we write `user = request.user` in our view.py files, where does that `user` attribute come from?  