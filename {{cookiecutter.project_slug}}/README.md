{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}

# {{ cookiecutter.project_name }}

{% if is_open_source %}
[![Pypi link](https://img.shields.io/pypi/v/{{ cookiecutter.project_slug }}.svg)](https://pypi.python.org/pypi/{{ cookiecutter.project_slug }})
{%- endif %}

{% if cookiecutter.add_pyup_badge == 'y' %}
[![Pyup](https://pyup.io/repos/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/shield.svg)](https://pyup.io/repos/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/)
{% endif %}

{{ cookiecutter.project_short_description }}

## Table of Content:

- [Intallation](#installation)
- [Usage](#usage)
- [TODO](#todo)
- [Contributing](#contributing)
- [Credits](#credits)

## Installation


```batch

    $ pip install {{ cookiecutter.project_slug }}
```

This is the preferred method to install {{ cookiecutter.project_name }}, as it will always
install the most recent stable release.

If you don't have [pip](https://pip.pypa.io) installed, this 
[Python installation guide](http://docs.python-guide.org/en/latest/starting/installation/) 
can guide you through the process.

## Usage

TODO


## TODO

- [ ] Update readme.


## Contributing

Contributions are welcome, and they are greatly appreciated! Every little bit
helps, and credit will always be given.

You can contribute in many ways:

### Types of Contributions

#### Report Bugs

Report bugs at [here](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/issues).

If you are reporting a bug, please include:

* Your operating system name and version.
* Any details about your local setup that might be helpful in troubleshooting.
* Detailed steps to reproduce the bug.

#### Fix Bugs

Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
wanted" is open to whoever wants to implement it.

#### Implement Features

Look through the GitHub issues for features. Anything tagged with "enhancement"
and "help wanted" is open to whoever wants to implement it.

#### Write Documentation

{{ cookiecutter.project_name }} could always use more documentation, whether as part of the
official {{ cookiecutter.project_name }} docs, in docstrings, or even on the web in blog posts,
articles, and such.

##### Submit Feedback

The best way to send feedback is to file an [issue](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/issues).

If you are proposing a feature:

* Explain in detail how it would work.
* Keep the scope as narrow as possible, to make it easier to implement.
* Remember that this is a volunteer-driven project, and that contributions
  are welcome :)

### Get Started!

Ready to contribute? Here's how to set up `{{ cookiecutter.project_slug }}` for local development.

1. Fork the `{{ cookiecutter.project_slug }}` repo on GitHub.
2. Clone your fork locally:

```console
$ git clone git@github.com:your_name_here/{{ cookiecutter.project_slug }}.git
```

3. Install development dependencies:

    ```console
    $ cd {{ cookiecutter.project_slug }}/
    $ pip install -r requirements_dev.txt
    ```

4. Create a branch for local development::

    ```console
    $ git checkout -b name-of-your-bugfix-or-feature
    ```

    Now you can make your changes locally.

5. When you're done making changes, check that your changes pass flake8 and the
   tests, including testing other Python versions with tox::

   ```console
    $ flake8 src/{{ cookiecutter.project_slug }} tests
    $ python -m pytest
    ```

6. Commit your changes and push your branch to GitHub::

    ```console
    $ git add .
    $ git commit -m "Your detailed description of your changes."
    $ git push origin name-of-your-bugfix-or-feature
    ```

7. Submit a pull request through the GitHub website.


## Deploying


A reminder for the maintainers on how to deploy. Make sure all your changes are
committed (including an entry in HISTORY.md). Then update the version according
to semver. Then run:

```batch
$ git tag vX.X.X -m "Your message"
$ git push
$ git push --tags
```

The CI system will then deploy to PyPI if tests pass.  Contributions are
welcome, and they are greatly appreciated! Every little bit helps, and credit
will always be given.



## Credits

This package was created with Cookiecutter and the `odarbelaeze/cookiecutter-simple-pypackage` project template.

- [Cookiecutter](https://github.com/audreyr/cookiecutter)
- [odarbelaeze/cookiecutter-simple-pypackage](https://github.com/odarbelaeze/cookiecutter-simple-pypackage)
