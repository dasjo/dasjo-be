# dasjo-be

Requirements

* git - https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
* docksal - https://docksal.io/installation
* pantheon terminus - https://pantheon.io/docs/terminus/install

Setup

* git clone git@github.com:dasjo/dasjo-be.git
* fin drush bash
* terminus aliases
* cd das-be
* mkdir database_dumps
* composer install
* Set up web/sites/default/settings.local.php based on https://docs.docksal.io/tools/drupal/
* Set $settings['hash_salt'] based on terminus drush dasjo-be.dev -- ev 'return getenv("DRUPAL_HASH_SALT")'
* fin init
* http://dasjo-be.docksal should be available now

Update database from pantheon dev

* fin downloaddb


[![CircleCI](https://circleci.com/gh/dasjo/dasjo-be.svg?style=shield)](https://circleci.com/gh/dasjo/dasjo-be)
[![Dashboard dasjo-be](https://img.shields.io/badge/dashboard-dasjo_be-yellow.svg)](https://dashboard.pantheon.io/sites/c63ab8da-cec4-4d01-b9c0-198938b4328c#dev/code)
[![Dev Site dasjo-be](https://img.shields.io/badge/site-dasjo_be-blue.svg)](http://dev-dasjo-be.pantheonsite.io/)
