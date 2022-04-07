# Code Questions





## 2022-04-05 

1. 
2. BIG: how do we view Markdown file source from a webpage


## 2022-04-04 

1. When I follow the trace stack where are all these init files being kept? psycopg2 has one that causes an error in my application but I can't find it.

## 2022-04-04 

1. how many servers are there for an app like QuestionBox?
2. if we had pictures for a user or profile, do we store them in the db server?


## 2022-03-30 
1. If we don't use registration redux, do we still make a User class in Models from AbstractUser?
2. Should we start our project by creating a local postgres db and depoloying to a new Heroku db?
3. It doesn't seem like settings.py recognizes my environ import
    - SECRET_KEY not configured properly again.
4. auth.User clashes with models.User when I try to add. I really don't understand users lol.

## 2022-03-29 

1. See if Paul or one of the front end peeps knows: 
    - How do I make the colums in bulma stay the same size regardless of the number of elements in the row / grid?


## 2022-03-29 

## After class with Amy
1. My local development server is still running on 8000, is it reading my .env?
2. Find and solve local migration bug.. datetime.datetime etc
3. Wipe servers if not deployed? Need this alot lol
4. Where does Meta class comes from?
5. `from rest_framework import generics` does not seem to be recognized in my `snippets/views.py` or `snippets/urls.py`
6. where is `rest_framework` sourcecode?

   
## 2022-03-28 

- When do we use related names in models?  Does that only show up in the db gui?


## 2022-03-28

### General
- Is there a way to get class notes from `momentum-team-11.github.io` already in .md format?

### Documentation Q's

- Learning question: I want to create a radio for a boolean value in my form.
- I open django source code and search for the Class I want.
- class ModelForm is in models.py inside the django/forms directory.. so when we write from django import forms do we get access then to all 'modules' and classes within them? 
- class ModelForm inherits from BaseModelForm, so I go to that source
- I am assuming these are the list of all attributes and methods I can override.. so may not be a question here.  Use for a while and come back to.
- When I lookup `class BooleanField` it gives me a list of all the available fields and it looks like the template gives a true or false checkbox for model boolean fields.

## 2022-03-26

- Why does registration-redux direct me to '/accounts/login/habits' instead of just 'habits/'?

## 2022-03-25

- Tracing the file paths through the Django source code, `AppConfig` in django.apps is really a Class in the file `config.py` found by the path from the root of : `Django/django/apps/config.py`

- When we write `user = request.user` in our view.py files, where does that `user` attribute come from?  