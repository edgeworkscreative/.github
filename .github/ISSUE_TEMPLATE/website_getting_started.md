---
name: ⚙️ Dev Site Setup
about: Start a new development site
title: 'Start a new development site'
labels: project details
assignees: ''

---


## Getting Started

If you are the first developer on a new project, create an empty database for the development to take place on.

Either way, you'll need database connection credentials for your .env

To get started:

- [ ] Gather DB credentials (create new empty db, if needed)
- [ ] Set up your local environemnt incl .user.ini , web.config, autoload.php
- [ ] Set .env variables - check paths, email addresses, etc.
- [ ] Run Composer Install and Migrations
- [ ] Sync /uploads folder with team

Run composer and migrations by issuing these commands from a terminal window at the root of your project:

``` bash

    composer install

    php run_migrations.php run

```
