# PHP Setup (Using DDEV)

## Prerequisites
1. Make sure Docker is running.

## Installation Steps (One Time)
> Please note that the following actions need to be performed only once for this project.

Run below commands in sequence

```
mkdir project-name
cd project-name
```

```
ddev config --project-type=php --docroot=web --create-docroot
ddev start
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
1. [Setup a Project](https://ddev.readthedocs.io/en/stable/users/project)
