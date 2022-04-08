# Error List

This is an idea I'm trying out to create a bank of errors I've made so I can quickly access the solutions when I find them.

```shell pm makemigrations   ```        

```shell
 It is impossible to add the field 'created' with 'auto_now_add=True' to answer without providing a default. This is because the database needs something to populate existing rows.

 1) Provide a one-off default now which will be set on all existing rows
 2) Quit and manually define a default value in models.py.
Select an option: 2
```