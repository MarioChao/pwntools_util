# Test packages

Test with output

```sh
python -m pytest -s
```

# Build distribution files

Build package & generate distribution

```sh
python -m build
```

# Upload test package

Upload distribution to test server

```sh
twine upload --repository testpypi dist/*
```

Install package from test server

```sh
pip install --index-url https://test.pypi.org/simple/ --no-deps pwntools-util
```

# Upload real package

Upload distribution to PyPI

```sh
twine upload dist/*
```

Install package from test server

```sh
pip install pwntools-util
```
