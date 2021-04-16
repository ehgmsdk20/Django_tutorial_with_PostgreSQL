# Django_tutorial_with_PostgreSQL
prerequisite: PostgreSQL, Python
## 1. How to create Database in postgreSQL
Install the PostgreSQL in [PostgreSQL official site](https://www.postgresql.org/).   
Then, run the SQL Shell(psql) and enter password.   
Command line will change into "postgres=#".    
1. Create Database and access

```
CREATE DATABASE <databasename_used_in_Django>;
\c <databasename_used_in_Django>
```
Command line will change into "<databasename_used_in_Django>=#".    
2. Create User
```
CREATE ROLE <username> with login password <password>;
```
3. Set the Database(Optional)
```
ALTER role <username> SET client_encoding to 'utf-8';   
ALTER role <username> SET timezone to 'Asia/Seoul';   
```
4. Grant privileges to user   
```
GRANT all privileges ON database <databasename> to <username>;
GRANT all privileges ON database <test_databasename> to <username>;
```
