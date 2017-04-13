=============================
{{cookiecutter.project_name}}
=============================

{{cookiecutter.description}}

.. image:: https://readthedocs.org/projects/{{cookiecutter.repo_name}}/badge/?version=latest
  :target: https://readthedocs.org/projects/{{cookiecutter.repo_name}}/?badge=latest
.. image:: https://travis-ci.org/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}.svg?branch=master
  :target: https://travis-ci.org/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}
.. image:: https://circleci.com/gh/coecms/ARCCSSive.svg?style=shield
  :target: https://circleci.com/gh/coecms/ARCCSSive
.. image:: http://codecov.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/coverage.svg?branch=master
  :target: http://codecov.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}?branch=master
.. image:: https://landscape.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/master/landscape.svg?style=flat
  :target: https://landscape.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/master
.. image:: https://codeclimate.com/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/badges/gpa.svg
  :target: https://codeclimate.com/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}
.. image:: https://badge.fury.io/py/{{cookiecutter.repo_name}}.svg
  :target: https://pypi.python.org/pypi/{{cookiecutter.repo_name}}
.. image:: https://circleci.com/gh/{{cookiecutter.github_account}}/{{cookiecutter.package_name}}.svg?style=svg
  :target: https://circleci.com/gh/{{cookiecutter.github_account}}/{{cookiecutter.package_name}}

.. content-marker-for-sphinx

---
Install
---

Conda install::

    conda install -c {{cookiecutter.github_account}} {{cookiecutter.package_name}}

Pip install (into a virtual environment)::

    pip install {{cookiecutter.repo_name}}

---
Develop
---

Development install::

    git checkout https://github.com/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}
    cd {{cookiecutter.repo_name}}
    conda env create -f conda/dev-environment.yml
    source activate {{cookiecutter.package_name}}-dev
    pip install -e '.[dev]'

Run tests::

    py.test

Build documentation::

    python setup.py build_sphinx
