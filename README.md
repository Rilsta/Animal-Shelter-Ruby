# Animal-Shelter-Ruby
**by Riley Starnes and Jeff Seymour**

## Project
Build an Animal Shelter website where users can view animals for adoption. Use CRUD functionality 
with Ruby, Sinatra, and psql to manipulate data in a Postgres database. Practice RESTful routing and
Behavior Driven Development.

## Installation
Clone the Repository
* `git clone https://github.com/Rilsta/Animal-Shelter-Ruby.git`
* Navigate to project directory

Install the ruby gems
* `$bundle install`

Set up the database by running the following:
* `$psql`
* `CREATE DATABASE animal_shelter`
* `\c animal_shelter`
* `CREATE TABLE animals (id serial PRIMARY KEY, name varchar, gender varchar, admittance_date timestamp, type varchar, breed varchar, customer_id int)`
* `CREATE TABLE customers (id serial PRIMARY KEY, name varchar, phone varchar, animal_type_pref varchar, breed_preference varchar)`

For testing, stay in psql and run the following
* `CREATE DATABASE animal_shelter_test WITH TEMPLATE animal_shelter`
* exit psql and run `$rspec`

To view:
* `ruby app.rb`
* Open a web browser and navigate to localhost:4567

## License
MIT License 2016
