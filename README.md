# esteemed-screening-d8

As the Esteemed Screening Department scales to accommodate more candidates, we
expect to receive a lot of Drupal 8 and Drupal 9 code examples for review.

This repository uses Acquia BLT to provide a convenient method for rapidly
evaluating code samples for adherence to Drupal coding standards.

Each candidate's code sample will also be saved in the repository as a feature
branch, in case a client asks to see a sample of a candidate's work.

## Quick start

* Clone this repository to your local workstation.

```
$ git clone git@github.com:hotwebmatter/esteemed-screening-d8.git
```

To spin up a local development environment using Lando:

* Copy the `lando.local.settings.php` file over the `local.settings.php` file:

```
cp docroot/sites/default/settings/lando.local.settings.php docroot/sites/default/settings/local.settings.php
```

* Execute `lando start` to spin up the Docker containers:

```
lando start
```

* Use 'lando drush` to install the default Drupal 8 installation profile:

```
lando drush site-install standard --db-url=mysql://drupal8:drupal8@database/drupal8 -y
```

You will now be able to preview the candidate's code sample at the following URLs:
- http://screening-d8.lndo.site/
- https://screening-d8.lndo.site/

## Screening process

Documentation forthcoming on the screening process, but in a nutshell:

* Create a new git branch for the candidate's code sample:

```
$ git checkout -b candidate_name
```

* Save their code in the appropriate location for custom module or theme.

* Use BLT to run tests on their code. [README-BLT](./README-BLT.md)

## Local dev preview environment

* Forthcoming: local dev preview, possible deploy to screening environment.
