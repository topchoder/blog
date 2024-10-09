pip install django
django-admin startproject blog_project
cd blog_project
python manage.py startapp blog
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',
    }
}
python manage.py makemigrations
python manage.py migrate
