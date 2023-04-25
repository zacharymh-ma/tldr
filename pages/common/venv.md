# venv

> Create lightweight virtual environments in python.
> More information: <https://docs.python.org/3/library/venv.html>.

- Check python venv module is installed properly:

`python -m venv --help`

- install python venv module:

`sudo apt-get install -y python3-venv`

- Create a python virtual environment:

` python -m venv {{path/to/virtual_environment}}`

- Activate the virtual environment (Linux and Mac OS):

`source {{path/to/virtual_environment}}/bin/activate`

- Activate the virtual environment (Windows):

`{{path\to\virtual_environment}}\Scripts\activate.bat`

- Deactivate the virtual environment:

`deactivate`

- Create virtual environment with a custom prompt name, otherwise the name will be the same as project root directory:

`python -m venv --prompt {{PROMPT}} {{path/to/virtual_environment}}/.venv`

- Create virtual environment with access of system site-packages (python version environment if pyenv is in use):

`python -m venv --system-site-packages {{PROMPT}} {{path/to/virtual_environment}}/.venv`

- Create virtual environment without pip, useful when using a dependency manager (e.g. poetry, pipenv, etc):

`python -m venv --without-pip {{path/to/virtual_environment}}/.venv`
