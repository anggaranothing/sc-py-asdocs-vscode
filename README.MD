# sc-py-asdocs-vscode

Converts `asdocs.txt` into `as.predefined` for use in [sashi0034/angel-lsp](https://github.com/sashi0034/angel-lsp) VSCode extension.

## Requirements

* [Python >=3.9](https://www.python.org/downloads/)
* [Poetry](https://python-poetry.org/docs/#installation)

## How to Get `asdocs.txt`

* Open a Terminal/Command Prompt,
* Execute this command: `steam -applaunch 225840 -as_outputdocs asdocs +map _server_start`
* Wait until map is loaded, and then close the game,
* A file named `asdocs.txt` should be created in Sven Co-op game mod folder ("`Sven Co-op/svencoop`"),
* Copy `asdocs.txt` file from that folder into this directory,
* Run the Python script.

## How to Extract Script Base Classes from Game

* Copy "extras/extract_asbaseclasses.cfg" file into "Sven Co-op/svencoop_addon" folder,
* Open a Terminal/Command Prompt,
* Execute this command: steam -applaunch 225840 +exec extract_asbaseclasses.cfg
* Wait until a new game has been closed automatically,
* A file named "console-XXXX-XX-XX.log" should be created in Sven Co-op game folder,
* Copy that file into "sc-py-asdocs-vscode" folder,
* Run the Python script.

## How to Run

* Open a Terminal/Command Prompt at this directory,
* Execute this command:
```bash
poetry update
poetry run python build.py asdocs.txt as.predefined console-XXXX-XX-XX.log
```
