# {{cookiecutter.project_slug}}

![tests](https://github.com/{{cookiecutter.github_user}}/{{cookiecutter.project_name}}/workflows/main/badge.svg)
![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
![Black](https://img.shields.io/badge/code%20style-black-000000.svg)

# What is it?

TODO

# Development

## Install (dev mode)

```console
$ make install
```

[Set up `pre-commit` hooks](https://pre-commit.com/).


## Usage

* Auto-format: `make format`
* Run static checkers: `make static_checks`
* Freeze the local env into `test_requirements` (say, after installing new deps): 
  `make freeze_requirements`.

## Issues

Please raise [here](https://github.com/{{cookiecutter.github_user}}/{{cookiecutter.project_name}}/issues).

## Credits

This project was generated from [@elvijs](https://github.com/elvijs)'s 
[Minimal Python Cookiecutter](https://github.com/elvijs/cookiecutter-minimal-python) template.
