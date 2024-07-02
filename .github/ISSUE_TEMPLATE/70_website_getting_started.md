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

## Housekeeping

If this is a re-design project it will be necessary to capture existing URLs into a 301. You Check sitemap files on old sites or Search Console for existing known URLs.

- [ ] Capture all known page URLs to a Sheet and record in Project Details issue.

