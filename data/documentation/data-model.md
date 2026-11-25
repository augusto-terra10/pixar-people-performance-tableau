# Data Model

## Overview

The dashboard combines information about Pixar films, creative contributors, box office performance, awards, public response, and film genres.

The source files currently included in the project are:

- `Pixar Films.csv`
- `Pixar People.csv`
- `Box Office.csv`
- `Academy Awards.csv`
- `Public Response.csv`
- `Genres.csv`

## Data Sources

| Dataset | Purpose |
|---|---|
| Pixar Films | Film-level information used to describe and identify Pixar titles |
| Pixar People | Creative contributors and their roles in Pixar films |
| Box Office | Box office performance associated with films |
| Academy Awards | Academy Award information associated with films or contributors |
| Public Response | Audience/public response information associated with films |
| Genres | Genre classifications associated with films |

## Relationships and Analysis

The dashboard uses film titles/film identifiers to connect film-level information across the relevant datasets. Contributor records connect people and creative roles to the films they worked on.

The main analysis paths are:

1. Select a creative role to filter the contributor analysis.
2. Select a contributor in the scatter plot to filter the film poster gallery.
3. Hover over a film poster to display the contributors associated with that film.

## Notes

- Confirm the exact join keys and relationship cardinality in the Tableau data model before documenting them as definitive.
- Contributor data may contain multiple rows for the same person when that person has multiple roles or film credits.
- Review source data licensing and redistribution permissions before committing CSV files to a public GitHub repository.
