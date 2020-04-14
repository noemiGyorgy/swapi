release: python manage.py migrate
release: python manage.py loaddata planets.json
release: python manage.py loaddata people.json
release: python manage.py loaddata species.json
release: python manage.py loaddata transport.json
release: python manage.py loaddata starships.json
release: python manage.py loaddata vehicles.json
release: python manage.py loaddata films.json
web: gunicorn swapi.wsgi --log-file -
