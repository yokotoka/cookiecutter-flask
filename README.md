# cookiecutter-flask

A Flask template for [cookiecutter](https://github.com/audreyr/cookiecutter). (Supports Python ≥ 3.6)

[![Build Status](https://travis-ci.org/cookiecutter-flask/cookiecutter-flask.svg?branch=master)](https://travis-ci.org/cookiecutter-flask/cookiecutter-flask)
[![CalVer](https://img.shields.io/badge/calver-19.0.0-22bfda.svg)](http://calver.org)

## Use it now

### Docker **(This is the preferred method for creating a new project)**

```bash
# Basic usage (You will be prompted to provide basic information about your application)
$ bin/run-cookiecutter
    full_name [Steven Loria]:

# Additional arguments are available
$ bin/run-cookiecutter --help
    Usage: run-cookiecutter [OPTIONS]

Options:
    -b, --build    Build Docker image before running cookiecutter
    -t, --template Specify custom cookiecutter template via a URI to a git repo
                    e.g. https://github.com/cookiecutter-flask/cookiecutter-flask.git
                    Defaults to template in current working directory
    -h, --help     Show this message and exit
```

### Standard

If using standard instructions, Python ≥ 3.6 is required. A virtual environment is recommended (like `virtualenv`).

```bash
pip3 install cookiecutter
cookiecutter https://github.com/cookiecutter-flask/cookiecutter-flask.git
```

You will be asked about your basic info (name, project name, app name, etc.). This info will be used in your new project.

## Configure and Run

After you have generated the project code, a few more steps must be taken before your new app will run. The README of the generated project shows you how to configure and run the application. (You can see the [template README here](https://github.com/cookiecutter-flask/cookiecutter-flask/blob/master/%7B%7Bcookiecutter.app_name%7D%7D/README.md)).

## Features

- Bootstrap 4 and Font Awesome 4 with starter templates
- Flask-SQLAlchemy with basic User model
- Easy database migrations with Flask-Migrate
- Configuration in environment variables, as per [The Twelve-Factor App](https://12factor.net/config)
- Flask-WTForms with login and registration forms
- Flask-Login for authentication
- Flask-Bcrypt for password hashing
- Procfile for deploying to a PaaS (e.g. Heroku)
- pytest and Factory-Boy for testing (example tests included)
- Flask's Click CLI configured with simple commands
- CSS and JS minification using webpack
- npm support for frontend package management
- Caching using Flask-Cache
- Useful debug toolbar
- Utilizes best practices: [Blueprints](http://flask.pocoo.org/docs/blueprints/) and [Application Factory](http://flask.pocoo.org/docs/patterns/appfactories/) patterns

## Screenshots

![Home page](https://user-images.githubusercontent.com/2379650/45271508-917f1c00-b475-11e8-9153-7f7385707a8b.png "Home page")

![Home page](https://user-images.githubusercontent.com/2379650/45271517-a9ef3680-b475-11e8-8de6-fbf3d9cab199.png "Registration form")

## Inspiration

- [Structuring Flask Apps](http://charlesleifer.com/blog/structuring-flask-apps-a-how-to-for-those-coming-from-django/)
- [Flask-Foundation](https://github.com/JackStouffer/Flask-Foundation) by [@JackStouffer](https://github.com/JackStouffer)
- [flask-bones](https://github.com/cburmeister/flask-bones) by [@cburmeister](https://github.com/cburmeister)
- [flask-basic-registration](https://github.com/mjhea0/flask-basic-registration) by [@mjhea0](https://github.com/mjhea0)
- [Flask Official Documentation](http://flask.pocoo.org/docs/)

## License

MIT licensed.

## Changelog

See the [Changelog](CHANGELOG.md).
