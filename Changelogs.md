# Changelogs

# [v0.1.0] pytest & Improved getting numbers | 2025/09/16

Formatted the file structure to support [pytest](https://docs.pytest.org/en/stable/index.html).

Allowed number getter functions to retrieve **negative** numbers.

New `PwnUtil` features:
- `getAllNumbersFromLine()`


# [v0.0.2] Initial pwntools_util package | 2025/09/15

Uploaded the pwntools_util package to the Python Package Index (PyPI).

Included `PwnUtil` features:
- `connectRemote(host, port)`
- `connectLocal(path_to_file, path_to_interpreter="./.venv/bin/python")`
- `disconnect()`
- `getline(timeout=5)`
- `getuntil(data, timeout=5)`
- `getall(timeout=5)`
- `sendline(data)`
- `interactive()`
- `getNumberFromLine()`
- `getNumberListFromLine()`
