# {{ cookiecutter.project_name }}

## Introduction
{{ cookiecutter.description }}

## Installation

1. Install [poetry](https://python-poetry.org/docs/) in global environment

   ```sh
   sudo pip3 install poetry
   ```

2. Install [commitizen](https://commitizen-tools.github.io/commitizen/) and [pre-commit](https://pre-commit.com) in project path

   ```sh
   poetry install
   ```

3. Install the git hook scripts

   ```sh
   poetry run pre-commit install
   poetry run pre-commit install -t commit-msg
   ```

## Usage

1. Activate the virtual environment

   ```sh
   source ./.venv/bin/activate
   ```

2. Create new commit

   ```sh
   cz c
   ```

3. Bump semantic version and generate changelog based on the git log

   ```sh
   cz bump --changelog --yes
   ```
