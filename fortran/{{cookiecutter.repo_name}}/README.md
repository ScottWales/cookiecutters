# {{cookiecutter.repo_name}}

[![Documentation Status](https://readthedocs.org/projects/{{cookiecutter.repo_name}}/badge/?version=latest)](https://readthedocs.org/projects/{{cookiecutter.repo_name}}/?badge=latest)
[![Build Status](https://travis-ci.org/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}.svg?branch=master)](https://travis-ci.org/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}})
[![codecov.io](http://codecov.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}/coverage.svg?branch=master)](http://codecov.io/github/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}?branch=master)

{{cookiecutter.description}}

Build Instructions:
-------------------

Requires:
 * Fortran compiler
 * MPI library
 * pFUnit

To build & test:

    mkdir build && pushd build
    cmake ..
    make
    ctest

A Vagrantfile is provided to create a VM with the required dependencies:

    vagrant up
    vagrant ssh
    make
    ctest
