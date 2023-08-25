# Base Airflow

This repo contains a base airflow project that can be extended to be used as a full fledged airflow project.

## Prerequisite

- [pyenv](https://github.com/pyenv/pyenv)
- [Poetry](https://github.com/python-poetry/poetry)

## Installation

- This template is built using python `3.9.16` if you want to change the python version, please change it to [pyproject.toml](pyproject.toml#L11) and also in [settings.yaml](settings.yaml#L5)
- Install base dependencies by running the command `poetry install`. This will initiate a python 3.9.16 poetry environment and also install airflowctl
- Once initiated please use the poetry environment using `poetry shell`
- From inside the poetry shell in the root directory
  - Install the pre-commit hooks using the command `pre-commit install && pre-commit run --all`
  - Build the project using the command `cd airflow && airflowctl build && cd ..`
