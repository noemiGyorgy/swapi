release: python manage.py migrate
release: python manage.py createsuperuser
release: python manage.py loaddata people.json
web: gunicorn swapi.wsgi --log-file -
