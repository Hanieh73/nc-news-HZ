# Northcoders News API

## Husky

To ensure we are not commiting broken code this project makes use of git hooks. Git hooks are scripts triggered during certain events in the git lifecycle. Husky is a popular package which allows us to set up and maintain these scripts. This project makes use a _pre-commit hook_. When we attempt to commit our work, the script defined in the `pre-commit` file will run. If any of our tests fail than the commit will be aborted.

The [Husky documentation](https://typicode.github.io/husky/#/) explains how to configure Husky for your own project as well as creating your own custom hooks.\_

## Comments

As .env.\* is added to the .gitignore, anyone who wishes to clone this repo will not have access to the necessary environment variables. Therefore a developer must add two files separately as .env.test & .env.development with (PGDATABASE=<database_name_here>) in order to successfully connect to the two databases locally. The name of the databases can be taken from setup.sql
