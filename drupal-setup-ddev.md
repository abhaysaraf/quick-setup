# Drupal Setup (Using DDEV)

> Please note that the following actions need to be performed only once. In future, the same setup maybe useful while you setup other projects.

## Prerequisites
No prerequisites as such.

## Installation Steps
Run below commands in sequence.

```
mkdir project-name
cd project-name
```

```
ddev config --project-type=drupal10 --docroot=web --create-docroot
ddev start
```

```
ddev composer create "drupal/recommended-project:^10"
ddev composer require drush/drush
```

```
ddev drush site:install -y
ddev drush uli
ddev describe
ddev launch
```

## References
1. [Quick-start Drupal CMS](https://ddev.readthedocs.io/en/stable/users/quickstart/#drupal)
