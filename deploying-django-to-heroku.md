# Deploying a Django App to Heroku
From class: [Deploying Postgres Database Locally](https://momentumlearn.notion.site/Using-Postgres-Locally-6d24cd1ea8854eabb875023d6696fba9)

Class notes: [Deploying Postgres Django app to Heroku](https://momentumlearn.notion.site/Deploying-a-Django-App-to-Heroku-81488333c03445539bfc7eb3c1691ed0#df1b110251304048849f96ca9453ed04)

## Setup from class
`brew install postgresql`


Run this command to verify that postgresql is running
 ```sh 
brew services list
 ```

This command will then start postgresql on your computer
```sh
brew services start postgresql
```

Once you have postgresql running on your computer, you can start to make databases

## Create new database

For every database you will need to run through this process.
```sh
createuser -d <username> 
createuser -d habbit-tracker 
createdb -U <username> <dbname>
createdb -U habbit-tracker habbit-tracker
```

Show list of all of databases
```sh
psql -l
```

Connect an 'adapter' to allow django ORM to communicate with Postgres Database on Heroku
```sh
pipenv install psycopg2-binary
```
You can check this was installed correctly by looking for it in the pipfile and will be listed as `psycopg2-binary = "*",`

In the .env file, add:
```sh
DATABASE_URL=postgres://<username>:@127.0.0.1:5432/<dbname>
```

Migrate to new heroku database
```sh
python manage.py migrate
pmm
```

The gui we'll use for our Postgres databases is `Postico`