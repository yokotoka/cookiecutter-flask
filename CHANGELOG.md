# Changelog

### 19.0.0 (11/26/2019)

- Add support for running app in Docker
- Upgrade Python versions to >= 3.6
- Upgrade Node versions to >- 10
- Validate Python module names
- Add support for Heroku deployments
- Replace deprecated `flask-webpack` with `flask-static-digest`
- Increase linting (`isort`, cyclomatic complexity)
- Refactor webpack config
- Refactor `commands.py`


### 18.0.0 (09/09/2018)

- Use CalVer (`YY.MINOR.MICRO`).
- Upgrade to Bootstrap 4. Thanks [@adawalli](https://github.com/adawalli) and [@Hiyorim](https://github.com/Hiyorimi).
- Use environment variables for configuration.
- Add support for Pipenv.
- Upgrade Python and Node dependencies.

### 0.13.0 (06/25/2017)

- Use webpack for building front-end assets. Front-end dependencies are
  installed with NPM. Remove Flask-Assets and bower.json. Thanks
  [@wroberts](https://github.com/wroberts).

### 0.12.0 (11/06/2016)

- Update Python dependencies.

### 0.11.1 (11/06/2016)

- Correctly pass first parameter to `Flask` according to the 0.11 [docs](http://flask.pocoo.org/docs/0.11/api/#application-object). Thanks [@aliavni](https://github.com/aliavni).
- Remove setuptools and wheel as dependencies to fix deployment on Heroku. Thanks [@Cabalist](https://github.com/Cabalist).
- Make User.password a Binary field for compatibility with new versions of bcrypt. Thanks again [@Cabalist](https://github.com/Cabalist).

### 0.11.0 (09/10/2016)

- Use the FLASK_DEBUG system environment variable, instead of MYFLASKAPP_ENV, to control different configs for development and production environments

### 0.10.1 (08/28/2016)

- Fix `invoke test` command.

### 0.10.0 (08/28/2016)

- Update to Flask 0.11.
- Use Click instead of Flask-Script for CLI commands.

### 0.9.0 (03/06/2016)

- Update stale requirements.
- Add CSRF protection.
- Run `lint` command on Travis builds.
- Test against Python 3.5.

### 0.8.0 (11/09/2015)

- Update stale requirements.
- Add `lint`, `clean`, and `urls` management commands.
- Add isort.

Thanks @andreoliw for these contributions.

### 0.7.0 (04/14/2015)

- Update extension import style to flask_* as per [mitsuhiko/flask#1135](https://github.com/mitsuhiko/flask/issues/1135).
- Update stale requirements (Werkzeug, Flask-WTF, WTForms, Flask-Bcrypt, Flask-DebugToolbar, Flask-Migrate, Bootstrap, jQuery). Thanks @bsmithgall for notifying me of the critical patch to Flask-Migrate.

### 0.6.0 (12/01/2014)

- Test the cookiecutter on Travis. Thanks @joshfriend.
- Update stale requirements (Flask-WTF, Flask-Migrate, Flask-DebugToolbar)

### 0.5.0 (09/29/2014)

- Fix .travis.yml.
- Update stale requirements (Flask-WTF, WTForms, Flask-SQLAlchemy, jquery, Bootstrap)

### 0.4.3 (07/27/2014)

- Add `BaseFactory` class.
- Add compat.py module.
- Tests pass on Python 3.

### 0.4.2 (07/27/2014)

- Update factories to factory-boy >= 2.4.0 syntax.
- Update stale requirements.

### 0.4.1 (06/07/2014)

- Update stale requirements (Werkzeug 0.9.6, WTForms 2.0)
- Fix unmatched div tag in home.html (thanks [@level09](https://github.com/level09))

### 0.4.0 (04/19/2014)

- Add ReferenceCol for less verbose foreign key columns.
- Add SurrogatePK mixin for adding integer primary key to a model.
- Add base Model class that has CRUD convenience methods.
- Fix setting BCrypt encryption complexity. Tests are much faster.
- Add Role model to show ReferenceCol usage.
- Switch to pytest.
- Upgrade all out-of-date requirements.
- More test examples.
- Remove "year" from cookiecutter.json (just change LICENSE if necessary).

### 0.3.2 (02/26/2014)

- Fix static assets.

### 0.3.1 (02/20/2014)

- Update default year in cookiecutter.json. Thanks @Omeryl
- Correct testing of redirects in webtests. Thanks @Widdershin
- Fix POST action in nav form. Thanks @Widdershin.
- Update Bootstrap (3.1.1) and jQuery (2.1.0)
- Optional support for bower.
- Minified assets aren't used in dev environment.

### 0.3.0 (12/08/2013)

- More modular organization: each blueprint contains its own view, models, and forms in a directory. There is still a single directory for templates and static assets.
- Use Flask-Bcrypt for password hashing.
- Flask-Login for authentication.
- Simple test setup. Just create a subclass of `DbTestCase`.
- Flask-Testing support.
- Use Factory-Boy for test factories.
- Use WebTest for functional testing.
- Add Flask-Debugtoolbar.
- Migrations using Flask-Migrate.
- Caching using Flask-Cache.
- Add error page templates (404, 401, 500)
- Add Font Awesome 4.0.3 for icons.

### 0.2.0 (09/21/2013)

- Add manage.py script
- Add Flask-Assets for CSS and JS bundling+minification
- Use different configs for development and production environments, controlled by the MYFLASKAPP_ENV system environment variable
- Use Blueprints and application factory pattern. The `simple` branch does not use these.

### 0.1.0 (08/20/2013)

- First iteration
- Bootstrap 3 final
- Working User model and registration
