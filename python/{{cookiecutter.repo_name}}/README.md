# {{cookiecutter.project_name}}

{{cookiecutter.description}}

[![Documentation Status](https://readthedocs.org/projects/{{cookiecutter.repo_name}}/badge/?version=latest)](https://readthedocs.org/projects/{{cookiecutter.repo_name}}/?badge=latest)
[![Build Status](https://travis-ci.org/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}.svg?branch=master)](https://travis-ci.org/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}})
[![codecov.io](http://codecov.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/coverage.svg?branch=master)](http://codecov.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}?branch=master)
[![Code Health](https://landscape.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/master/landscape.svg?style=flat)](https://landscape.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/master)
[![Code Climate](https://codeclimate.com/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/badges/gpa.svg)](https://codeclimate.com/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}})
[![PyPI version](https://badge.fury.io/py/{{cookiecutter.repo_name}}.svg)](https://pypi.python.org/pypi/{{cookiecutter.repo_name}})

Build Instructions:
-------------------

Pip install (into a virtual environment):

    pip install {{cookiecutter.repo_name}}

or
    
    pip install git+https://github.com/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}

or (for development)

    git checkout git+https://github.com/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}
    cd {{cookiecutter.repo_name}}
    pip install -e '.[dev]'
