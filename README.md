# Ramadan Time — central data

Public data for the [Ramadan Time](https://github.com/saadh393/RamadanTime) Android app: Bangladesh Hijri date corrections and the list of Islamic occasions.

The app downloads [`data.json`](data.json) about once a day from:

```
https://raw.githubusercontent.com/saadh393/ramadan-time-data/main/data.json
```

The format and the rules a file must follow are documented in the app repository's `_docs/central-data.md`. An invalid file is ignored by the app, which keeps its previous copy.

## Publishing a change

1. Edit `data.json` (for example, add a Hijri correction when Bangladesh's moon-sighting committee announces a month start that differs from Umm al-Qura).
2. Commit to `main`. The app picks it up within a day.
3. Copy the same file into the app's `app/src/main/assets/central-data.json` before the next release, so new installs start with it.
