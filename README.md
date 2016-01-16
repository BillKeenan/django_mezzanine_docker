# django_mezzanine_docker
Django Mezzanine CMS Starter Project using Docker & Postgresql

# Dependencies
- Python 3.4.x
- Django 1.8.x
- Mezzanine 4.0.1
- Postgresql 9.5

# Usage

### Build
    docker-compose build
    
### Start Container
    docker-compose up
    
### Create Database and Site
The first time you start this you need to create the database by running:
 
    docker-compose run mezz python manage.py createdb
    
### Go to site
[http://localdocker:8902](http://localdocker:8902)

In my local environment I set `localdocker` to resolve to the ip address of my docker VM. Change this as appropriate.

# Notes

### SECRET_KEY
Make sure you change/set this in `app/settings.py` file.

# References

- [Mezzanine CMS](http://mezzanine.jupo.org/)