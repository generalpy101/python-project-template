# Python Project Template

This is a template which I intend to use in my Python projects.

Final directory structure will be:

```bash
{{cookiecutter.src_name}}
    ├── init_hooks.sh
    ├── lint.py
    ├── pyproject.toml
    ├── tests
    │   └── test_pass.py
    └── {{cookiecutter.project_name}}
        ├── __init__.py
        └── main.py
```

`{{cookiecutter.src_name}}` will be replaced by the name you provide to your source directory. `{{cookiecutter.project_name}}` will be replaced by your project name. `tests` contains tests for your code.

## Installation

To use this template, you first have to run some commands. This project was created on Ubuntu Linux and assumes that you have linux too because some commands might or might not be same in other OSes(especially windows).

First and foremost, create a virtual environment. This whole template will run as module and uses `pyproject.toml` to become installable as a module so you need to have a virtual environment. [Read more here](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/)

So to create a virtual environment, in your terminal, execute:

```bash
python -m venv <virtual_env_name>
```

Then activate it with:

```bash
source ./<virtual_env_name>/bin/activate
```

After that, to install this project as a module, execute:

```bash
pip install -e .[dev]
```

Read more about `-e` option [here](https://stackoverflow.com/questions/35064426/when-would-the-e-editable-option-be-useful-with-pip-install). Read more why I used `[dev]` [here](https://stackoverflow.com/questions/62408719/download-dependencies-declared-in-pyproject-toml-using-pip).

Now you can import file and packages from `src` directory anywhere in your virtual enviroment. Try importing `main.py` anywhere in your project.


### Contribution

I am not a python genius and this is the reason I created this repo, so that I can save some time. Please consider contributing to it to improve its quality, Thanks in advance.
