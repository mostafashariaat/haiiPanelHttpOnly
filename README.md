httponly panel

Run project:

1-install all packages of the project by running "pip install -r requirements.txt" in a terminal

2-create a postgresql database and a superuser in postgresql. Then all you need to do is give your database user access rights to the database you created :

Install Postgresql on your operating system, then connect to a PSL database and run this query to create a database.

"CREATE DATABASE dbname;"

Then to give access to the superuser you have been created, run this query :

"GIVE THE USER ALL ACCESS TO THE DATABASE dbname;"

To give better information about how to configure PostgreSQL, read the below link.

https://www.digitalocean.com/community/tutorials/how-to-use-postgresql-with-your-django-application-on-ubuntu-20-04

3-fill.env-sample file with valid information and then rename.env-sample to.env

4-run python manage.py migrate and python manage.py makemigrations in terminal

5-in haiiPanelHttpOnly.settings.py find CORS_ALLOWED_ORIGINS and then put the port of the front-end framework or library (react,angular,vue,...) run