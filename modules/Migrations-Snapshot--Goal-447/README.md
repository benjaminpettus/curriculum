# Migrations Snapshot (447)

## Skills

- Can describe what a SQL migration is
- Can describe why we need SQL migrations
- Can take an existing SQL schema, and convert them into migrations
- Can create automated scripts to `reset`, `migrate`, and `seed` a SQL database

## Description

You will start by cloning a starter app which already has a database schema defined. You will then modify the project such that the schema will be managed by database migrations.

### Setting Up Your Snapshot

1. Fork & clone the [SQL Migrations Starter Repo](https://github.com/GuildCrafts/sql-migrations-snapshot)
1. Follow the install instructions in the README of the starter repo

## Specifications

- Use the [node-pg-migrate](https://github.com/theoephraim/node-pg-migrate) library to add migrations to your project
- Using the library above to create a migration for the SQL defined in the `src/db/schema/schema.sql` file
- An npm script `db:migrate` exists which migrates the db to the latest migration
- An npm script `db:init` exists which creates the database and migrates the database to the latest migration
- An npm script `db:migration:create` exists which lets you create a new migration
- Create a migration for a table called `user`. Table should contain the following fields
  - id
  - first_name
  - last_name
  - email
