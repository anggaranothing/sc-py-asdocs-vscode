# sc-py-asdocs-vscode

Converts `asdocs.txt` into `as.predefined` for use in [sashi0034/angel-lsp](https://github.com/sashi0034/angel-lsp) VSCode extension.

## Requirements

* [Python >=3.9](https://www.python.org/downloads/)
* [Poetry](https://python-poetry.org/docs/#installation)

## How to Run

* Retrieve `asdocs.txt` file by running Sven Co-op with this command line added:
```
-dev -as_outputdocs asdocs
```

* Copy `asdocs.txt` file into this directory,

* Open terminal/command prompt at this directory,

* Execute this command:
```bash
poetry update
poetry run python build.py asdocs.txt as.predefined
```
