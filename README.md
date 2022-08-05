haii panel httponly
Run project: 
1- install all package of project by run "pip install -r requirements.txt" in terminal

2- create postgresql database and superuser in postgresql then all you need to do is give your database user access rights to the database you created : 
first install postgresql in your OS then connect to psql database after that run this query for creating database
"CREATE DATABASE dbname;" 
then to give access to superuser you have been created run this query : 
GRANT ALL PRIVILEGES ON DATABASE dbname TO user;
to give better information about how configure postgresql read below link: 
https://www.digitalocean.com/community/tutorials/how-to-use-postgresql-with-your-django-application-on-ubuntu-20-04

3- fill .env-sample file by valid information and then rename .env-sample to .env

4- in haiiPanelHttpOnly.settings.py find CORS_ALLOWED_ORIGINS and then put port of front-end framework or library (react,angular,vue,...) run  

