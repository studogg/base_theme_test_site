# NAL Drupal 8 Base Site Profile
This repository is a collection of dependencies and configuration intended for
quickly creating new Drupal 8 websites at NAL. It will contain all of the
commonly-required modules and settings that are needed by our websites.  The
structure of the files is built upon the [Composer template for Drupal
projects](https://github.com/drupal-composer/drupal-project).  The initial site
configuration was started from the D8 Minimal profile, which allows you to
install the site from existing configuration, a feature that was added in
Drupal 8.6.0.
## Project Contacts
* Project owner: [David Cameron](mailto:david.cameron@ars.usda.gov) @dcameron
* Project manager: [Sherry Panzer](mailto:sherry.panzer@ars.usda.gov) @spanzer
* Technical contact: [David Cameron](mailto:david.cameron@ars.usda.gov)
  @dcameron
## Usage Instructions
Downloading the project must be done with ```git clone```. Then the ```.git```
directory must be manually deleted in order to disassociate the new project
from this base profile.  In the future, we may try to streamline these
instructions be making it possible to use the ```composer create-project```
command to automatically perform those same tasks.

Set up a database for your new website.  Then execute the following commands
from the command line.
1. ```git clone git@github.com:isdapps/drupal-base-profile.git PROJECT_DIR```
2. ```cd PROJECT_DIR```
3. ```rm -rf .git```
4. ```composer install```
5. ```git init```
6. ```git add .```
7. ```git commit -m "Added base profile files."```
8. ```drush site-install --existing-config```

The ```composer install``` command will overwrite the ```README.md``` file with
a standard template for NAL Drupal projects.  You will need to customize the
README with your new project's info after the installation is complete.

The ```drush site-install``` command will prompt you for your database name and
credentials.

