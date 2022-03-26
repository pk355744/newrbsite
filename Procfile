web: gunicorn wrappers.wsgi:application --log-file - --log-level debug
python manage.py collectstatic --noinput
manage.py migrate
web: python manage.py runserver 0.0.0.0:$PORT
release: python manage.py migrate