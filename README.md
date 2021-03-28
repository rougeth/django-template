# Django Project Template

## How to use

```bash
$ django-admin startproject --name Procfile,setup.cfg --template https://github.com/rougeth/django-template/archive/master.zip new_django_project .
```

## Features

- Heroku Ready
  > [Heroku](https://www.heroku.com/) is a container-based cloud Platform as a Service (PaaS). It's easy to use, manage and scale. Is it expensive? Depend of the use case, but if you consider the time you won't spend configuring and maintaining a server, probably not.
- `accounts` Django with a single empty model `Userl`:

    > If you’re starting a new project, it’s highly recommended to set up a custom user model, even if the default User model is sufficient for you. This model behaves identically to the default user model, but you’ll be able to customize it in the future if the need arises.

    [https://docs.djangoproject.com/en/3.1/topics/auth/customizing/#using-a-custom-user-model-when-starting-a-project](https://docs.djangoproject.com/en/3.1/topics/auth/customizing/#using-a-custom-user-model-when-starting-a-project)

### Configuration files
- `Procfile` - Define how Heroku should run the application (Django/Gunicorn at this case) - [https://devcenter.heroku.com/articles/procfile](https://devcenter.heroku.com/articles/procfile)
- `runtime.txt` - Define which Python version to run the application - [https://devcenter.heroku.com/articles/python-runtimes](https://devcenter.heroku.com/articles/python-runtimes)

### Dependencies

- `python-decouple` - Config settings like `DEBUG`, `ALLOWED_HOSTS` or `SECRECT_KEY` in a environment variable or `.env`file when running locally - [https://pypi.org/project/python-decouple/](https://pypi.org/project/python-decouple/)
- `psycopg2-binary` - PostgreSQL database adapter for Python - https://pypi.org/project/psycopg2-binary/
- `dj-database-url` - Database configuration for Django in a single url - [https://pypi.org/project/dj-database-url/](https://pypi.org/project/dj-database-url/)
- `whitenoise` - Serve static files directly from Django - [http://whitenoise.evans.io](http://whitenoise.evans.io/)
- `gunicorn` - WSGI HTTP Server for Python - [https://gunicorn.org/](https://gunicorn.org/)

#### Development

- `ipython` - Python shell (manage.py shell as well) with super powers - [https://pypi.org/project/ipython/](https://pypi.org/project/ipython/)
- `ipdb` - Python pdb debugger integrated with `ipython` - [https://pypi.org/project/](https://pypi.org/project/ipython/ipdb/)

#### Test & Code style

- `pytest` - The best testing framework for Python - [https://docs.pytest.org/en/stable/](https://docs.pytest.org/en/stable/)
- `black` - Code formatter - [https://pypi.org/project/black/](https://pypi.org/project/black/)
- `isort` - Utility to sort imports alphabetically and automatically separated into sections - [https://pypi.org/project/isort/](https://pypi.org/project/isort/)
