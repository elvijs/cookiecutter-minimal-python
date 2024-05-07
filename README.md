# cookiecutter-minimal-python

Minimal Python repo cookiecutter.

Sets up `pyproject.toml` and a Makefile that covers install, 

## Design decisions

* The key functionality is in a single location - the `Makefile`.
* The user manages the venv and use whatever they want (that is, no `poetry` or similar).
  - We define the project dependencies in `pyproject.toml` and 
    provide a frozen test environment via `test_requirements.txt` 
* We set up productivity tools like `black`, `mypy`, `pylint` and `isort`.
  - We use [the Google `pylintrc`](https://github.com/google/styleguide/blob/gh-pages/pylintrc),
    but change the indentation to 4 spaces.
* We set up `pytest` with code coverage checks.

If you like more batteries included, then 
[the hypermodern cookiecutter](https://github.com/cjolowicz/cookiecutter-hypermodern-python/tree/main)
might be better suited.

# Usage

## Prerequisites

`pip install cookiecutter`

## Create a repo

`cookiecutter gh:elvijs/cookiecutter-minimal-python`


# FAQ

* Why no `poetry`?
  - It adds unnecessary complexity that I've found a pain to debug.
    Project requirements and `test_requirements.txt` combo seems to be 
    a simple yet powerful solution for early projects.
* Why `pylint`?
  - It's slow, but powerful and I like static checkers to do 
    as much heavy lifting as possible.
    [`ruff`](https://docs.astral.sh/ruff/) is really exciting and 
    a good candidate for switchover once 
    [it reaches feature parity](https://github.com/astral-sh/ruff/issues/970). 
