# Changelogs

# [v0.2.1] connectLocal argument update | 2025/09/22

Updated the arguments for `PwnUtil.connectUtil()`, allowing more variety of processes to run:
- Old: `connectLocal(path_to_file, path_to_interpreter="./.venv/bin/python")`
- New: `connectLocal(self, argv = None, *args, **kwargs)`


# [v0.2.0] Refactor: modules & number functions | 2025/09/22

Refactored global constants and functions into modules under `pwntools_util.util`:
- `type utilities` => `.util.type_convert`
- `string utilities` => `.util.string_getter`
- text colors `_COLORS` => `.util.text_colors`

Refactored getters for `int` numbers:
- `getNumberFromLine()` => `getFromLine_Int()`
- `getAllNumbersFromLine()` => `getAllFromLine_Int()`
- `getNumberListFromLine()` => `getListFromLine_Int()`

New `PwnUtil` features (`float` getters):
- `getFromLine_Float()`
- `getAllFromLine_Float()`
- `getListFromLine_Float()`


# [v0.1.1] Connect Remote Parameters | 2025/09/19

Added the arguments for `pwn.remote()` to `PwnUtil.connectRemote()`.


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
