rails -T

# Explain what, when and an use case example for each of the following rails db tasks:

rails db:create # Creates the database from DATABASE_URL or config/database.yml for the current RAILS_ENV (use db:create:all to create all databases in the config). Without RAILS_ENV or when RAILS_ENV is development, it defaults to ...
rails db:drop # Drops the database from DATABASE_URL or config/database.yml for the current RAILS_ENV (use db:drop:all to drop all databases in the config). Without RAILS_ENV or when RAILS_ENV is development, it defaults to droppi...
rails db:environment:set # Set the environment value for the database
rails db:fixtures:load # Loads fixtures into the current environment's database
rails db:migrate # Migrate the database (options: VERSION=x, VERBOSE=false, SCOPE=blog)
rails db:migrate:down # Runs the "down" for a given migration VERSION
rails db:migrate:redo # Rolls back the database one migration and re-migrates up (options: STEP=x, VERSION=x)
rails db:migrate:status # Display status of migrations
rails db:migrate:up # Runs the "up" for a given migration VERSION
rails db:prepare # Runs setup if database does not exist, or runs migrations if it does
rails db:reset # Drops and recreates the database from db/schema.rb for the current environment and loads the seeds
rails db:rollback # Rolls the schema back to the previous version (specify steps w/ STEP=n)
rails db:schema:cache:clear # Clears a db/schema_cache.yml file
rails db:schema:cache:dump # Creates a db/schema_cache.yml file
rails db:schema:dump # Creates a database schema file (either db/schema.rb or db/structure.sql, depending on `config.active_record.schema_format`)
rails db:schema:load # Loads a database schema file (either db/schema.rb or db/structure.sql, depending on `config.active_record.schema_format`) into the database
rails db:seed # Loads the seed data from db/seeds.rb
rails db:seed:replant # Truncates tables of each database for current environment and loads the seeds
rails db:setup # Creates the database, loads the schema, and initializes with the seed data (use db:reset to also drop the database first)
rails db:structure:dump # Dumps the database structure to db/structure.sql
rails db:structure:load # Recreates the databases from the structure.sql file
rails db:version # Retrieves the current schema version number
