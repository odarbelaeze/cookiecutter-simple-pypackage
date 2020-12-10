# cookiecutter-simple-pypackage
   

[Cookiecutter](https://github.com/audreyr/cookiecutter) simple template for a Python package.


## Features

* Testing setup with [pytest](https://docs.pytest.org/)
* Auto-release to [PyPI](https://pypi.python.org/pypi) when you push a new tag to master.
* Command line interface using Click (optional)


## Quickstart

Install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher):

```bash

    $ pip install -U cookiecutter
```

Generate a Python package project:

```bash
    cookiecutter https://github.com/odarbelaeze/cookiecutter-simple-pypackage
```

Then:

* Create a repo and put it there.
* Install the dev requirements. (`pip install -r requirements_dev.txt`) not needs for virtualenv.
* [Register](https://packaging.python.org/distributing/#register-your-project) your project with PyPI.
* Start developing your package.
* Release your package by pushing a new tag to master.


For more details, see the cookiecutter-pypackage [tutorial](https://cookiecutter-pypackage.readthedocs.io/en/latest/tutorial.html).


## Not Exactly What You Want?

Don't worry, you have options:

### Similar Cookiecutter Templates


* [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage): The original pypackage.

* [Nekroze/cookiecutter-pypackage](https://github.com/Nekroze/cookiecutter-pypackage): A fork of `audreyr/cookiecutter-pypackage` with a PyTest test runner,
  strict flake8 checking with Travis/Tox, and some docs and `setup.py` differences.

* [ardydedase/cookiecutter-pypackage](https://github.com/ardydedase/cookiecutter-pypackage): A fork with separate requirements files rather than a requirements list in the ``setup.py`` file.

* Also see the [network](https://github.com/audreyr/cookiecutter-pypackage/network) and [family tree](https://github.com/audreyr/cookiecutter-pypackage/network/members) for this repo. (If you find
  anything that should be listed here, please add it and send a pull request!)

### Fork This / Create Your Own


If you have differences in your preferred setup, I encourage you to fork this
to create your own version. Or create your own; it doesn't strictly have to
be a fork.

* Once you have your own version working, add it to the Similar Cookiecutter
  Templates list above with a brief description.

* It's up to you whether or not to rename your fork/own version. Do whatever
  you think sounds good.

### Or Submit a Pull Request


I also accept pull requests on this, if they're small, atomic, and if they
make my own packaging experience better.

