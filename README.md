# myLogs

- __Description__ : personal general purpose logging system
- __Tech stack__ : svelte, MySQL
- __Roll no__ : CS19B1042, CS19B1065, CS19B1055
- __Course__ : CS309 - Database Management System Laboratory

## Idea

To build a logging system that is simple and flexible.

### Overview

- Log is considered as the primary entity in our system.
- Our system can have any number of category types that have any number of categories whose semantics are upto the user.
- Tag is a simple short text whose semantics is upto the user.
- Category (_not category type_) is a tag prefixed with special characters. The special character prefix is considered
  as a unique identifier of a category type.
- Each log could be associated with any number of tags except exactly one category tag per category type.
- Log can also be not associated with any category tag.

### Features

- User could filter by tags and time.
- Each tag is colored, also uniquely as much as possible.

## Architecture

### Components

- MySQL
- Server
- Svelte web app

### Tables in Database
- logs(id, text, timestamp)
- tags(log_id, label)
