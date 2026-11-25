# Data Model

## Overview

`Pixar Films.csv` is the central table in the Tableau data model. It is connected to five other datasets.

## Relationships

| Connected dataset | Relationship with `Pixar Films.csv` |
|---|---|
| `Academy Awards.csv` | One-to-many |
| `Box Office.csv` | One-to-one |
| `Genres.csv` | One-to-many |
| `Pixar People.csv` | One-to-many |
| `Public Response.csv` | One-to-one |

In other words, one Pixar film can have multiple Academy Award records, genre records, and people/contributor records. Each film has one corresponding record in the Box Office dataset and one corresponding record in the Public Response dataset.

## Model Structure

```text
Pixar Films
├── Academy Awards       (one-to-many)
├── Box Office           (one-to-one)
├── Genres               (one-to-many)
├── Pixar People         (one-to-many)
└── Public Response      (one-to-one)
```

## Dashboard Analysis

The model supports the dashboard's main interactions:

1. Select a creative role to explore contributors.
2. Select a contributor in the scatter plot to filter the film poster gallery.
3. Hover over a film poster to view the creative contributors associated with that film.

