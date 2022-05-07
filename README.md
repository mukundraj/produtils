
## Link for packaging instructions

https://packaging.python.org/en/latest/tutorials/packaging-projects/

## Test deployment commands summary

```
python3 -m pip install --upgrade build
python3 -m build
python3 -m pip install --upgrade twine
python3 -m twine upload --repository testpypi dist/*
python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps produtils-mukundraj
```


## Production deployment commands summary

- Remove username suffix from package name in cfg file
- clean dist folder

```
python3 -m pip install --upgrade build
python3 -m build
python3 -m twine upload dist/*

```

## For installing

```
python3 -m pip install produtils
```
