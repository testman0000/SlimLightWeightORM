# Project Overview

Couldn't find a lightweight easy to use ORM for PHP that wasn't connected to a MVC, so I made one.  This Lightweight ORM for PHP allows the quick setup of models and relationships and easy query building.

# ORM

## Naming Conventions

Tables and models need names that match.  This can be changed in the config file.

The **primary key** of a table should be the table name followed by "_id". Ex: A table named *wizard* should have a primary key of *wizard_id*.  Similar to the @JoinColumn annotation in hibernate.


## Associations

Supported associations:

- has many through
- belongs to
- has many


When setting associations up, the association name is the model name, not the table name. For **has many** associations, the model name is pluralized.

## Hooks

ORM provides a series of hooks to process data before and after events. Currently those are:

- before save
- after save
- before update
- after update
- before destroy
- after destroy

