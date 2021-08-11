# billing-app-backend : expenditures microservice

## Project description
Repository for expenditures microservice

## Branch Naming

Same as billing-app/README.md

## Running server

### With docker :: TODO
Follow these steps

1- TODO

### Local - No docker

Follow these steps

1- Download postgres
2- Install it
3- Initialize the postgres server
  
  $ pg_ctl -D 'C:/Program Files/PostgreSQL/13/data' start
    -D: set the directory of the PGDATA file

4- Create billing user

  $ npm run create-user (place the password you put in the installaion process)
  
It is created with a superuser called postgres. If you dont have it, you should create id. The password is the one you set. Not password in this case

5- Change password

  $ npm run change-password

This will alter the password of the previously created role to 'password'. It will used the postgres role mentioned in item (4). You should used the same password used in that item

6- Create the database

  $ npm run create-db

7- Run migrations

  $ npm run migrate-up

8- Initialize the server
 
  Inside __./src__

  $ npm run start