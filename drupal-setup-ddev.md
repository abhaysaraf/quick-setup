# Drupal Setup (Using DDEV)

## Prerequisites
1. Make sure Docker is running.

## Installation Steps (One Time)
> Please note that the following actions need to be performed only once for this project.

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

## Work Resumption
> Regular commands to execute when resuming work on this project.

```
cd project-name
ddev start
ddev describe
ddev launch
```

## References
1. [Quick-start Drupal CMS](https://ddev.readthedocs.io/en/stable/users/quickstart/#drupal)
