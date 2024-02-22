# Todo-List-PDHT

Todo List App with Django, HTMX, Tailwind and PostgreSQL

## How to install

To install run

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## How to run

To run server run once

```bash
source .venv/bin/activate
python manage.py tailwind install
python manage.py tailwind build
curl -oL todo_list/static/htmx.min.js https://unpkg.com/htmx.org
python manage.py collectstatic
python manage.py migrate
```

Finally run

```bash
python manage.py runserver
```

Note: _remember to create a .env file or set the good environment variables_

## Environment

This are the environment variables you need to set

```bash
DEBUG=True # or False
SECRET_KEY=[KEY] # a complicated KEY to django to use
DB_NAME=todolist # name of the database
DB_USER=todolist # name of the user
DB_PASSWORD=todolist # password of the user
DB_HOST=localhost # host of the database
DB_PORT=5432 # port of the database
```
