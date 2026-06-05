# open-football

> A curated map of open football (soccer) data: free datasets and exports, plus the scrapers and tooling to use them.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](LICENSE)

If you want to start working with football data and don't want to pay for it, there is far more out there than people realise. This list grew out of the running notes kept while building [the Reep Register](https://github.com/withqwerty/reep), an open identity layer for football data. Access is sometimes just about knowing what exists and how to find the right pieces you need.

Everything here is open: released by the provider, publicly dumped, or open source. Licences vary and are noted where they matter. **This list does not endorse scraping in violation of any site's terms of service.**

One honest gap worth naming: genuinely open event or tracking data from Africa, Asia, and South America barely exists. The Dynasty Scouting League release and openfootball's results are rare exceptions. Contributions that fill that frontier are especially welcome — see [Contributing](#contributing).

## Contents

- [Event data](#event-data)
- [Tracking data](#tracking-data)
- [Results and fixtures](#results-and-fixtures)
- [Fantasy and ID maps](#fantasy-and-id-maps)
- [Stats and ratings](#stats-and-ratings)
- [Scrapers and collection](#scrapers-and-collection)
- [Loaders, models and tooling](#loaders-models-and-tooling)
- [Visualisation](#visualisation)
- [Identity and cross-provider mapping](#identity-and-cross-provider-mapping)
- [Wikidata](#wikidata)
- [Video and assets](#video-and-assets)
- [Learning and references](#learning-and-references)
- [Licence glossary](#licence-glossary)

## Event data

- [StatsBomb Open Data](https://github.com/statsbomb/open-data) - Free event data across 20+ competitions, men's and women's, including historical men's World Cups (1958, 1962, 1970, 1974, 1986, 1990) plus 2018 and 2022 (with 360 data), the Women's World Cups (2019 and 2023), and five women's leagues. Custom attribution licence.
- [Wyscout — Pappalardo dataset](https://figshare.com/collections/Soccer_match_event_dataset/4415000) - Public Wyscout event data for the 2017/18 big-five leagues plus the 2018 World Cup and Euro 2016 (~1,941 games), by Pappalardo et al. (Nature Scientific Data, 2019). CC BY 4.0. [koenvo's repackage](https://github.com/koenvo/wyscout-soccer-match-event-dataset) restructures it as kloppy-loadable JSON.
- [Impect Open Data](https://github.com/ImpectAPI/open-data) - Bundesliga 2023/24 sample with packing, packing-xG and possession value (pxT); loadable via kloppy.
- [Dynasty Scouting League 2024](https://github.com/Afriskaut/dynasty-scouting-league-2024-open-data) - Event data, lineups and match metadata from the 2024 Dynasty Scouting League, in JSONL. Apache 2.0.
- [wosostats](https://github.com/amj2012/wosostats) - Hand-logged women's match event data from video (USWNT, NWSL, 2016 onward). Community-collected, now largely dormant. GPL-3.0.

## Tracking data

- [SkillCorner Open Data](https://github.com/SkillCorner/opendata) - Broadcast tracking and physical data for 10 A-League 2024/25 matches, with off-ball runs and phases of play. MIT.
- [Metrica Sports Sample Data](https://github.com/metrica-sports/sample-data) - Anonymised, synchronised tracking and event data for 3 matches in CSV, EPTS and JSON formats.
- [IDSSE-data](https://github.com/spoho-datascience/idsse-data) - Synchronised TRACAB tracking and DFL event data for 7 Bundesliga / 2. Bundesliga matches, from German Sport University Cologne. CC BY 4.0.
- [PFF FC 2022 World Cup](https://www.blog.fc.pff.com/blog/pff-fc-release-2022-world-cup-data) - Broadcast tracking, event data and play-by-play grades for all 64 matches of the 2022 men's World Cup; free on access request, loadable via kloppy.
- [Last Row](https://github.com/Friends-of-Tracking-Data-FoTD/Last-Row) - Hand-collected 2D player and ball tracking (20fps) of 19 Liverpool goal sequences. Permissive but unlicensed (credit the source).
- [Alfheim / Tromsø IL (Simula)](https://datasets.simula.no/alfheim/) - ZXY 20Hz player tracking plus stitched panorama broadcast video for 3 Tromsø IL home matches (2013). Free for research, citation required.
- [SoccerMon](https://zenodo.org/records/10033832) - GPS positional data plus athlete wellness and load reports from the Norwegian women's Toppserien across two seasons. CC BY 4.0.

## Results and fixtures

- [football-data.co.uk](https://www.football-data.co.uk/) - Results, match stats, and opening/closing betting odds in CSV/Excel across ~25 leagues, updated weekly.
- [footballcsv](https://github.com/footballcsv) - League results in clean, public-domain CSV across England, Spain, Germany, Austria, MLS and more. CC0.
- [football.json (openfootball)](https://github.com/openfootball/football.json) - Public-domain fixtures and results in JSON for the major European leagues, 2010/11 onward. CC0.
- [openfootball/world](https://github.com/openfootball/world) - Results for African (Egypt, Morocco, Algeria, Nigeria) and Asian (China, Japan) leagues in the openfootball text format. CC0.
- [openfootball/south-america](https://github.com/openfootball/south-america) - Brazilian, Argentine and Colombian league results in the openfootball text format. CC0.
- [openfootball/worldcup](https://github.com/openfootball/worldcup) - Every men's World Cup from 1930 to 2026 (including the 2026 fixtures) in the openfootball text format. CC0.
- [schochastics/football-data](https://github.com/schochastics/football-data) - 1.2M+ match results across 207 domestic leagues and 20 international tournaments (1888–2023), in parquet. ODC-BY.
- [international_results](https://github.com/martj42/international_results) - Every men's full international result since 1872 (49,000+ matches), plus shootouts and goalscorers. CC0.
- [engsoccerdata](https://github.com/jalapic/engsoccerdata) - English top-four-tier results from 1888 plus other leagues and competitions, as an R package and CSVs. Non-commercial use with citation.
- [Fjelstul English Football Database](https://github.com/jfjelstul/englishfootball) - 208,028 Premier League and EFL matches (1888–2024), with appearances and standings, in CSV and R. CC BY-SA 4.0.
- [Fjelstul World Cup Database](https://github.com/jfjelstul/worldcup) - Comprehensive men's and women's World Cup database: matches, goals, bookings and squads. CC BY-SA 4.0.
- [English Women's Football (EWF) Database](https://github.com/probjects/ewf-database) - Women's Super League (from 2011) and Championship (from 2014) matches, appearances and standings. CC BY-SA 4.0.
- [European Soccer Database](https://www.kaggle.com/datasets/hugomathien/soccer) - SQLite database of 25,000+ matches with events, lineups (X/Y), FIFA player and team attributes, and bookmaker odds across 11 European leagues (2008–2016). ODbL.
- [BrazilianFootball/Data](https://github.com/BrazilianFootball/Data) - ~11,000 Brazilian matches scraped from official CBF match dockets, Série A–D and Copa do Brasil (2013–2025). MIT.

## Fantasy and ID maps

- [Fantasy-Premier-League](https://github.com/vaastav/Fantasy-Premier-League) - Historical FPL data from 2016/17 in CSV, with Python scrapers; updated a few times per season. Non-standard licence.
- [FPL-ID-Map](https://github.com/ChrisMusson/FPL-ID-Map) - Crosswalk from FPL player IDs to Opta, FBref, Transfermarkt, Understat and WhoScored.

## Stats and ratings

- [FBref](https://fbref.com/) - Detailed match, player, and team statistics for hundreds of competitions; every table on the site exports to CSV.
- [Understat](https://understat.com/) - Shot-level data with xG for the top six European leagues; every table can be exported to CSV.
- [Club Elo](http://clubelo.com/) - Daily Elo ratings for European clubs back to 1939, with a free, keyless CSV API (http only).
- [American Soccer Analysis](https://www.americansocceranalysis.com/) - Free public app and API for advanced MLS, NWSL and USL metrics (xG, goals added/g+, xPass).

## Scrapers and collection

- [soccerdata](https://github.com/probberechts/soccerdata) - Python package scraping Club Elo, ESPN, FBref, football-data.co.uk, Sofascore, SoFIFA, Understat and WhoScored into tidy DataFrames. Apache 2.0.
- [ScraperFC](https://github.com/oseymour/ScraperFC) - Python package scraping Capology, Club Elo, FBref, Sofascore, Transfermarkt and Understat. GPL-3.0.
- [worldfootballR](https://github.com/JaseZiv/worldfootballR) - The canonical R scraper for FBref, Transfermarkt and Understat. Archived September 2025 but still on CRAN and widely used. MIT.
- [itscalledsoccer](https://github.com/American-Soccer-Analysis/itscalledsoccer) - Official Python and R client for the American Soccer Analysis API. MIT.
- [nwslR](https://github.com/adror1/nwslR) - R package consolidating NWSL player, team and match data. GPL-3.0.

## Loaders, models and tooling

- [kloppy](https://github.com/PySport/kloppy) - Standardises loading and modelling of event and tracking data across 16+ providers (StatsBomb, Stats Perform/Opta, Wyscout, Sportec, Metrica, SkillCorner, Tracab, Second Spectrum, PFF, Hawk-Eye, and more). BSD-3.
- [floodlight](https://github.com/floodlight-sports/floodlight) - High-level Python framework for loading and analysing tracking and event data across many providers. MIT.
- [databallpy](https://github.com/Alek050/databallpy) - Python library to load and synchronise event and tracking data, with built-in pressure, xG and xT models. MIT.
- [socceraction](https://github.com/ML-KULeuven/socceraction) - SPADL and Atomic-SPADL action representations plus the xT and VAEP action-value models (maintenance mode).
- [soccer_xg](https://github.com/ML-KULeuven/soccer_xg) - Train and analyse expected-goals models on Opta, Wyscout and StatsBomb data. Apache-2.0.
- [unravelsports](https://github.com/UnravelSports/unravelsports) - Python toolkit turning tracking data into graphs (GNNs), with pressing intensity and formation detection. MPL-2.0.
- [penaltyblog](https://github.com/martineastwood/penaltyblog) - Python modelling toolkit: Dixon-Coles and Bayesian goal models, team ratings, expected threat, and scrapers. MIT.

## Visualisation

- [mplsoccer](https://github.com/andrewRowlinson/mplsoccer) - Pitch plotting and football visualisation for matplotlib, with multiple pitch types, radars, heatmaps and StatsBomb loaders (Python). MIT.
- [ggsoccer](https://github.com/Torvaney/ggsoccer) - ggplot2 pitch plotting with multiple provider coordinate systems (R). MIT.
- [d3-soccer](https://github.com/probberechts/d3-soccer) - D3 plugin for pitches, heatmaps and event visualisation (JavaScript/TypeScript). BSD-3.
- [Campos](https://github.com/withqwerty/campos) - React component library for football charts, with adapters for common providers (the web/TypeScript counterpart to mplsoccer + kloppy).

## Identity and cross-provider mapping

- [The Reep Register](https://github.com/withqwerty/reep) - Canonical identity layer mapping players, teams, and coaches across 40+ providers, anchored to stable Wikidata IDs.
- [FPL-ID-Map](https://github.com/ChrisMusson/FPL-ID-Map) - FPL-to-provider ID crosswalk (also listed under Fantasy and ID maps).

## Wikidata

- [Wikidata dumps](https://dumps.wikimedia.org/wikidatawiki/entities/) - Full entity dumps (JSON, N-Triples, Turtle), which include football entities and cross-provider IDs.
- [QuickStatements](https://quickstatements.toolforge.org/) - Batch-edit Wikidata via simple text commands, useful for contributing football IDs back.

## Video and assets

- [SoccerNet](https://www.soccer-net.org/) - Large-scale benchmark and annual challenge for soccer video understanding across ~13 tasks (action spotting, tracking, re-identification, jersey numbers, calibration, captioning, game-state reconstruction), over 550 broadcast games. Labels are open; the raw broadcast video requires signing an NDA.
- [SoccerNet DevKit](https://github.com/SilvioGiancola/SoccerNetv2-DevKit) - Maintained development kit for the SoccerNet tasks and challenges (supersedes the original CVPR'18 code).
- [3D Shot Posture Dataset](https://github.com/calvinyeungck/3D-Shot-Posture-Dataset) - 2D and 3D body-pose keypoint annotations of shot movements (CVPR 2024). Apache-2.0.
- [football-logos](https://github.com/Leo4815162342/football-logos) - 3,000+ club and national-team crests in SVG and PNG, organised by country and tournament.

## Learning and references

- [football_analytics (Edd Webster)](https://github.com/eddwebster/football_analytics) - A vast curated index of football analytics resources; the unofficial bible.
- [The Analytics Handbook (Devin Pleuler)](https://github.com/devinpleuler/analytics-handbook) - Hands-on football analytics tutorials and notebooks that bundle open data. MIT.
- [PySport open-source index](https://opensource.pysport.org/?sports=Soccer) - A directory of ~44 open-source soccer tools; the best single index of the ecosystem.
- [awesome-soccer-analytics](https://github.com/matiasmascioto/awesome-soccer-analytics) - A sister curated list of soccer analytics resources (Euro-centric). CC0.
- [RSSSF](https://www.rsssf.org/) - The Rec.Sport.Soccer Statistics Foundation: a volunteer-maintained archive of historical tables, results and records worldwide. The deepest historical reference on the web (browse-only, no bulk export).
- [Nutmeg](https://nutmeg.withqwerty.com) - AI skills and an MCP server that make coding agents fluent in football data and providers.
- [football-docs](https://github.com/withqwerty/football-docs) - Searchable provider documentation (qualifier IDs, coordinate systems, metric definitions) as an MCP server.

## Contributing

PRs welcome. To add a source:

1. It must be **open** — released by the provider, a public dump, or open source. No links that require breaching a site's terms of service to use, and no data restricted to registered competition participants.
2. Add it to the most fitting section, in the format `- [Name](url) - One-line description ending in a period.`
3. Keep descriptions factual and concise (what the data is, its coverage and licence — not marketing).
4. Run a quick check that the link resolves.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guidelines.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)

To the extent possible under law, [withqwerty](https://www.withqwerty.com) has waived all copyright and related or neighbouring rights to this curated list (the list itself; the linked resources carry their own licences). See [LICENSE](LICENSE).

## Licence glossary

A plain-English guide to the licences referenced above. This is a friendly summary, not legal advice — read the actual licence before you rely on it, especially for commercial use.

**Data licences** (cover the datasets)

- **CC0 / public domain** — Do whatever you like, no strings attached. Crediting the source is polite but not required. The most permissive option.
- **CC BY 4.0** (Attribution) — Free to use, including commercially, as long as you credit the source.
- **CC BY-SA 4.0** (Attribution-ShareAlike) — Free to use commercially, but you must credit the source *and* release anything you build from it under the same licence. "Share-alike" means passing the same freedom on.
- **ODC-BY** (Open Data Commons Attribution) — Like CC BY, but written specifically for databases: use freely, just credit the source.
- **ODbL** (Open Database License) — Like CC BY-SA for databases: use and adapt freely, but credit the source and share any adapted database under the same terms.

**Software licences** (cover the tools, scrapers, and libraries)

- **MIT** — Do almost anything (use, modify, sell); just keep the original copyright notice. The most common permissive licence.
- **BSD-3-Clause** — Practically the same as MIT, with one extra rule: you can't use the original authors' names to promote your version.
- **Apache-2.0** — Permissive like MIT, plus an explicit patent grant that protects you from patent claims by contributors. Common for larger projects.
- **MPL-2.0** (Mozilla Public License) — A middle ground: you can use it inside closed-source software, but changes to the MPL-licensed files themselves must stay open.
- **GPL-3.0** — "Copyleft": use and modify freely, but if you distribute software built on it, that whole work must also be open-sourced under the GPL. Good for keeping things open, restrictive if you want to keep your own code private.

**Other arrangements you'll see here**

- **Custom attribution licence** (e.g. StatsBomb) — Free to use, but on the provider's own terms — typically credit them, show their logo, and don't resell the data. Read their licence file.
- **Non-commercial, with citation** (e.g. engsoccerdata) — Free for research, learning, and personal projects, but not for commercial use, and you should cite it.
- **Non-standard or unstated licence** (e.g. Fantasy-Premier-League, Last Row) — No clear open licence attached. Usually fine for personal and research use with credit, but legally ambiguous for commercial use — ask the author if it matters.
- **Free for research, citation required** (e.g. Alfheim/Simula) — Open for academic and research use as long as you cite the dataset; commercial use may need permission.

One practical point: a dataset's licence covers the **data**, and a tool's licence covers the **code**. Using an open-source scraper (say, MIT-licensed) to pull data from a website does not give you any rights over that website's data — the source's own terms still apply.
