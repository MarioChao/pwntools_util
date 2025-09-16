Build package & generate distribution

```sh
python3 -m build
```

## Test package

Upload distribution to test server

```sh
twine upload --repository testpypi dist/*
```

Install package from test server

```sh
pip install --index-url https://test.pypi.org/simple/ --no-deps pwntools-util
```

# Real package

Upload distribution to PyPI

```sh
twine upload dist/*
```

Install package from test server

```sh
pip install pwntools-util
```
