# e-Liquid_Calculator

1. In order to load base.html from the base dir, you have to add 
'DIRS': [BASE_DIR / "templates"], to LIQUID_ROOT/settings.py TEMPLATES

2. We need to add static files directory in LIQUID_ROOT/settings.py

# Static files (CSS, JavaScript, Images)
# https://docs.djangoproject.com/en/4.2/howto/static-files/

STATIC_URL = 'static/'

# THIS STUFF HERE
STATICFILES_DIRS = [
    os.path.join(BASE_DIR, 'static'),
]

3. Downloaded template FOLDERS we copy/paste to our project's static folder

4. Downloaded template's index.html (home page, or landing page) content goes into our home.html or navigation.html, depending on the template

5. navigation.html has to load static {% load static %}
