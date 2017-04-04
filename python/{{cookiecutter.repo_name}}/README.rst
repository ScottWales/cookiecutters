=============================
{{cookiecutter.project_name}}
=============================

{{cookiecutter.description}}

.. image:: https://readthedocs.org/projects/{{cookiecutter.repo_name}}/badge/?version=latest
  :target: https://readthedocs.org/projects/{{cookiecutter.repo_name}}/?badge=latest
.. image:: https://travis-ci.org/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}.svg?branch=master
  :target: https://travis-ci.org/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}
.. image:: http://codecov.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/coverage.svg?branch=master
  :target: http://codecov.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}?branch=master
.. image:: https://landscape.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/master/landscape.svg?style=flat
  :target: https://landscape.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/master
.. image:: https://codeclimate.com/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/badges/gpa.svg
  :target: https://codeclimate.com/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}
.. image:: https://badge.fury.io/py/{{cookiecutter.repo_name}}.svg
  :target: https://pypi.python.org/pypi/{{cookiecutter.repo_name}}

.. content-marker-for-sphinx

------------------
Build Instructions
------------------

Pip install (into a virtual environment)::

    pip install {{cookiecutter.repo_name}}

or::
    
    pip install git+https://github.com/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}

or (for development)::

    git checkout https://github.com/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}
    cd {{cookiecutter.repo_name}}
    pip install -e '.[dev]'
