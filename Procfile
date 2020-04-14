release: python manage.py migrate
python manage.py dumpdata resources.planet > resources/fixtures/planets.json --indent 4
python manage.py dumpdata resources.people > resources/fixtures/people.json --indent 4
python manage.py dumpdata resources.species > resources/fixtures/species.json --indent 4
python manage.py dumpdata resources.starship > resources/fixtures/starships.json --indent 4
python manage.py dumpdata resources.vehicle > resources/fixtures/vehicles.json --indent 4
python manage.py dumpdata resources.transport > resources/fixtures/transport.json --indent 4
python manage.py dumpdata resources.film > resources/fixtures/films.json --indent 4
release: python manage.py loaddata planets.json
release: python manage.py loaddata people.json
release: python manage.py loaddata species.json
release: python manage.py loaddata transport.json
release: python manage.py loaddata starships.json
release: python manage.py loaddata vehicles.json
release: python manage.py loaddata films.json
web: gunicorn swapi.wsgi --log-file -
