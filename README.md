![alt text](https://ibb.co/M5RygGZ)


Front end -

run the command here from the /frontend and the react application will start.

npm start

Setup a Demo Backend
If you already have Cube.js Backend up and running you can skip this step

First, let’s install Cube.js CLI and create a new application with a Postgres database.

Command:

$ npm install -g cubejs-cli
$ cubejs create -d postgres backend

The Cube.js team host's a dump with sample data for tutorials. It is a simple “E-commerce database” with orders, products, product categories, and users tables.

$ curl http://cube.dev/downloads/ecom-dump.sql > ecom-dump.sql
$ createdb ecom
$ psql --dbname ecom -f ecom-dump.sql

Now that we have everything configured, the last step is to generate a Cube.js schema based on some of our tables and start the dev server.

$ cubejs generate -t line_items
$ npm dev
