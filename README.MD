# sc-py-asdocs-vscode

Converts `asdocs.txt` into `as.predefined` for use in [sashi0034/angel-lsp](https://github.com/sashi0034/angel-lsp) VSCode extension.

## Requirements

* [Python >=3.9](https://www.python.org/downloads/)
* [Poetry](https://python-poetry.org/docs/#installation)

## How to Run

```bash
poetry update
poetry run python build.py asdocs.txt as.predefined
```
