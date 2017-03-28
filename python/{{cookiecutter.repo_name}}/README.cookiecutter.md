Python Cookiecutter
===================

This cookiecutter makes use of Python Build Reasonableness,
https://docs.openstack.org/developer/pbr/#pbr, which has some nice features:

 * Version numbers is read from git tags
 * Nested packages are automatically found
 * Reads dependencies from requirements.txt

Setup
-----

Run cookiecutter:
```
cookiecutter /path/to/cookiecutters/python
```
 * project_name: Name of the project
 * repo_name: Name of the repository (no spaces)
 * package_name: Name of the Python package (Python token)
 * author_name: Your Name
 * author_email: Your Email
 * github_account: Github project (used to create badge links in the README)

Initialise the git repository:
```
cd {{cookiecutter.repo_name}}
git init .
git add .
git commit -m "Initial template"
```

Setup dev environment:
```
pip install -e .[dev]
```

Build documentation
```
python setup.py build_sphinx
```

Run tests
```
py.test
```

Upload to Github and set up services
```
git remote add origin git@github.com/{{cookiecutter.github_account}}/{{cookiecutter.repo_name}}
git push -u origin master
```

 * https://travis-ci.org/profile
 * https://readthedocs.org/dashboard/import/
 * https://landscape.io/repository/add
 * https://packaging.python.org/distributing/#uploading-your-project-to-pypi

To automatically deploy new tags to PyPI see https://docs.travis-ci.com/user/deployment/pypi/
