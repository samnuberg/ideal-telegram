# Ideal Telegram
This is a project for a online chat app. Mostly for exercise and because it's a fun project but who knows what's to come...

# Setup

Create a virtual environment to install dependencies in and activate it:
```bash
$ virtualenv venv
$ source venv/bin/activate
```

Duplicate the `env.local` file and rename it lo `.env`
<br />
<br />

#### Build an run docker:
```bash
(venv)$ docker-compose build
(venv)$ docker-compose up
```
Note the `(venv)` in front of the prompt. This indicates that this terminal session operates in a virtual environment set
<br />
<br />

Go to phpmyadmin `localhost:8082` and enter:
- Server: db
- Username: Check `.env` file
- Password: Check `.env` file

# Commands
#### Start development server:
```bash
(venv)$ docker-compose up
```

#### Make and run migrations:
```bash
(venv)$ python manage.py makemigrations
(venv)$ python manage.py migrate
```

## Running Tests
```bash
(venv)$ python manage.py test foo
(venv)$ python manage.py test foo.tests
(venv)$ python manage.py test foo.tests.FooTestCase
(venv)$ python manage.py test foo.tests.FooTestCase.test_foo_is_bar
```



