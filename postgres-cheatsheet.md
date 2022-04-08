# PostgreSQL commmand line utility (CLI) Cheatsheet

See a list of all the databases I've installed on my computer:
```shell
psql -l
```

<hr>

**See if Postgres is running:**
```shell
brew services list
```

<hr>

**Drop Database**
```shell
dropdb <databaseName>
```

<hr>

To **re-create a database after its been dropped**, the username will still be in the system.

Since I make the username and db name the same for simplicity on this setup I don't need to recreate a username. Just run:
```shell
createdb -U <username> <databaseName> 
```