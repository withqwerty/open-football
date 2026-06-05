# Contributing to open-football

Thanks for helping keep the map current. This list aims to be the place people land when they ask "where do I get football data without paying for it?"

## What belongs here

A resource qualifies if it is **open**:

- released by the provider themselves (e.g. StatsBomb Open Data), or
- a public data dump (e.g. Wikidata, RSSSF), or
- open-source tooling for collecting, loading, or modelling football data.

A resource does **not** belong here if using it requires breaching a website's
terms of service. This list documents where open data legitimately lives; it
does not endorse scraping against ToS.

## How to add a source

1. Fork the repo and edit `README.md`.
2. Put the entry in the most fitting section. If none fits, propose a new
   section in your PR.
3. Use this exact format:

   ```
   - [Name](https://url) - One-line description ending in a period.
   ```

4. Keep descriptions factual: what the data covers, its format or scope. No
   marketing language, no superlatives.
5. Check the link resolves and isn't already listed.
6. Keep entries alphabetical only where a section is already alphabetised;
   otherwise group by relevance.

## Updating an existing entry

Data sources change. If a dataset expands (new leagues, new seasons), is
relocated, or goes dead, a PR to update or remove the entry is very welcome.
Note what changed in the PR description.

## Quality bar

- One resource per line.
- Prefer the canonical/source link over a mirror (mirrors can be linked
  parenthetically, as with the Kaggle Transfermarkt mirror).
- If two entries overlap heavily, cross-reference rather than duplicate.

Open an issue first if you're unsure whether something fits.
