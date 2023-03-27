# Jobly Backend

This is the Express backend for Jobly, version 2. This project builds a RESTful API using Node.js, Express, and PostgreSQL.

## Table of Contents

- [Manual Installation](#manual-installation)
- [Commands](#commands)
- [Project Structure](#project-structure)
- [API Endpoints](#api-endpoints)

## Manual Installation

To clone the repo:

    git clone git@github.com:youssefdoss/express-jobly.git
    cd express-jobly

To install the dependencies:

    npm install

## Commands

To run this in development:

    node server.js

To run the tests:

    jest -i

## Project Structure

coverage\       # Coverage report
helpers\        # Helper for SQL and tokens
middleware\     # Authorization middleware
models\         # PSQL models
routes\         # Routes
schemas\        # Schemas

## API Endpoints

List of available routes:

**Auth routes**:\
`POST auth/token` - Get auth token
`POST auth/register` - Register

**Companies routes**:\
`POST companies` - Add company
`GET companies` - Get all companies
`GET companies/:handle` - Get company
`PATCH companies/:handle` - Update company
`DELETE companies/:handle` - Delete company

**Jobs routes**:\
`POST jobs` - Add job
`GET jobs` - Get all jobs
`GET jobs/:id` - Get job
`PATCH jobs/:id` - Update job
`DELETE jobs/:id` - Delete job

**Users routes**:\
`POST users` - Add user
`GET users` - Get all users
`GET users/:username` - Get user
`PATCH users/:username` - Update user
`DELETE users/:username` - Delete user
`POST users/:username/jobs/:id` - Apply to job