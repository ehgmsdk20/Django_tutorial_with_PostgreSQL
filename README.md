# Django_tutorial_with_PostgreSQL
## 1. How to create Database in postgreSQL
Install the PostgreSQL in [PostgreSQL official site](https://www.postgresql.org/).   
Then, run the SQL Shell(psql) and enter password.   
Command line will change into "postgres=#".    
1. Create Database

```
CREATE DATABASE <Databasename_used_in_Django>;
```
2. Create User
```
CREATE user <username> with password <password>;
```
3. Set the Database(Optional)
```
ALTER role root SET client_encoding to 'utf-8';   
ALTER role root SET timezone to 'Asia/Seoul';   
```
4. Grant privileges to user   
```
GRANT all privileges ON database <Databasename> to <username>;
```
