# Base Theme Test Site
This repository contains a Drupal 8 site profile, with dependencies and configuration necessary for developing a base theme.
## Installation Instructions
This project is designed to allow you to quickly install a fully-configured
copy of the website, with the exception of its content.

Set up a database for your copy of the website.  Then execute the following
commands from the command line.
1. ```git clone git@github.com:dcameron/base_theme_test_site.git PROJECT_DIR```
2. ```cd PROJECT_DIR```
3. ```composer install```
4. ```drush site-install --existing-config```
