# Postgre SQL
## Enter
```
sudo -u postgres psql
```
## Exit
```
\q
```
## Login
```
sudo -i -u postgres
```
## Logout
```
exit
```
## Create Database
```
CREATE DATABASE <db_name>;
```
## Database List
```
\l
```
## Create Role
```
CREATE ROLE <role_name> WITH ENCRYPTED PASSWORD '<password>';
```
## Grant
```
GRANT ALL PRIVILEGES ON DATABASE "<database_name>" to <username>;
```
## Change Password
```
\password
```
## Login Permission
```
ALTER ROLE "<role_name>" WITH LOGIN;
```
## Different Permisson on db to user
```
psql <db_name> -c "GRANT ALL ON ALL TABLES IN SCHEMA public to <user>;"
```
```
psql <db_name> -c "GRANT ALL ON ALL SEQUENCES IN SCHEMA public to <user>;"
```
```
psql <db_name> -c "GRANT ALL ON ALL FUNCTIONS IN SCHEMA public to <user>;"
```
