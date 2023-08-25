# Base Airflow

This repo contains a base airflow project that can be extended to be used as a full fledged airflow project.

## Prerequisite

- [pyenv](https://github.com/pyenv/pyenv)
- [Poetry](https://github.com/python-poetry/poetry)

## Installation

- **!!! Important. This project uses poe task runner to configure various tasks such as project install, docker build, docker-compose. Manually running this is not recommended beginners.**
- This template is built using python `3.9.16` if you want to change the python version, please change it to [pyproject.toml](pyproject.toml#L11) and also in [settings.yaml](settings.yaml#L5)
- Change the project name at [pyproject.toml](pyproject.toml#L2)
- Install base dependencies by running the command `poetry install`. This will initiate a python 3.9.16 poetry environment and also install airflowctl
- Once initiated please use the poetry environment using `poetry shell`
- From inside the poetry shell in the root directory
  - Install the pre-commit hooks and build the project using the command `poe setup-project`

## Running the airflow

### Using the airflowctl

- This project is built using airflowctl. Please refer to the original documentation on running it using airflowctl

### Using docker-compose

- Run the docker-compose script inside poetry shell using poe `poe docker-compose-up`
- Use the username and password as `airflow` in airflow authentication
