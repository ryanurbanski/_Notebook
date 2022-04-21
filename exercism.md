# Exercism Problems

Exercism is a fun way to practice and learn python, or really any language.

These setup notes were taken from:

[exercism setup tutorial](https://medium.com/@pathakanupam20/simple-guide-to-download-solve-submit-the-hello-world-python-exercise-at-exercism-io-2a0438d9f5d6)


## Running tests local

To run test the file `hello_world_test.py` for example we need to install pytest first.

```shell
pipenv install pytest pytest-cache
```

and can check it was installed properly with:


```shell
pytest --version
```

Once pytest is installed, pass the command:


```shell
python -m pytest hello_world_test.py
```


Once everything passes successfully you can submit with the command:

```shell
exercism submit hello_world.py
```








