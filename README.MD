## Django PostgreSQL Poetry Template

### Usage
- In `settings.py` set the database information under `DATABASES { ... }`:
  ```python
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql_psycopg2',
            'NAME': '<database_name>',
            'USER': '<database_username>',
            'PASSWORD': '<database_password',
            'HOST': '<database_hostname_or_ip_address>',
            'PORT': '<database_port>',
        }
    }
  ```
- Build the database migration and run it:
  ```python
    python manage.py makemigrations
    python manage.py migrate
  ```
- Create the superuser account:
  ```python
    python manage.py createsuperuser
  ```
- Run the Django server and test it:
  ```python
    python manage.py runserver 0.0.0.0:8000
  ```
