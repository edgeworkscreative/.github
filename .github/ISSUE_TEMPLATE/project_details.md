---
name: ▷ START HERE - PROJECT DETAILS AND SETUP
about: create a project details panel
title: ''
labels: project_details
assignees: ''

---


## [ PROJECT NAME ]

[ General Client / Project description here ]

## Project Deadlines & Billing

Project Deadline:

Harvest Project / Task:

## DEVELOPER INFO & RESOURCES

XD Design Document Link: [ insert link here ]

Client-Facing Project Sheet: [ insert link here ]

Staged Development Server URL: [ none yet ]

Live Website URL:

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
