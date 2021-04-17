# Django_tutorial_with_PostgreSQL
Tech Stack Used: Django, PostgreSQL, HTML, CSS     
prerequisite: PostgreSQL, Python    

## 1. Description
This project was created by referring to the Django tutorial documentation on the Django official site(https://docs.djangoproject.com/).   
I used PostgreSQL instead of sqlite.    

## 2. How to create Database in postgreSQL
Install the PostgreSQL in [PostgreSQL official site](https://www.postgresql.org/).   
Then, run the SQL Shell(psql) and enter password.   
Command line will change into "postgres=#".    
1. Create Database(and Database for testing) and access
```
CREATE DATABASE <databasename>;
\c <databasename>
```
Command line will change into "<databasename>=#".     
  
2. Create User
```
CREATE ROLE <username> with login password <password>;
```
3. Set the User
```
ALTER ROLE <username> CREATEDB
ALTER ROLE <username> SET client_encoding to 'utf-8';   
ALTER ROLE <username> SET timezone to 'Asia/Seoul';   
```
4. Grant privileges to user   
```
GRANT all privileges ON database <databasename> to <username>;
GRANT all privileges ON database <test_databasename> to <username>;
``` 

# 3. How to use
You can download my project through the command.   
```
https://github.com/ehgmsdk20/Django_tutorial_with_PostgreSQL.git           
```
Then, create venv and activate the virtual environment.(available from Python 3.3 or higher)   
```
python -m venv venv           
venv/Scripts/activate         
```
Install the libraries for this project.   
```
pip install -r requirements.txt        
```     
Finally, run the Flask web application.   
```     
cd tutorial
python manage.py runserver
```   
