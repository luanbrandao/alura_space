virtualenv venv
source venv/bin/activate

pip freeze
pip freeze > requirements.txt

django-admin startproject setup .

python manage.py runserver

pip install python-dotenv



python manage.py collectstatic