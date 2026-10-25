# Maven Graphic: College Football Résumé Rankings

A code recreation of the supplied college football rankings graphic, with real team logo assets. All 70 teams, rankings, and scores are transcribed from the reference, including ties and Northern Illinois at -0.36. These are reference scores, not live ratings.

![Rankings graphic](output/college-football-rankings.png)

## View the graphic

Download or clone the repository and open `output/college-football-rankings.html` in a modern browser. The HTML is standalone and works offline. It includes PNG and SVG download buttons and a drawer with the editable ranking data.

Generated files:

- `output/college-football-rankings.html`: standalone browser version
- `output/college-football-rankings.png`: 4096 × 2320 raster image
- `output/college-football-rankings.svg`: scalable graphic with outlined text

## Edit and rebuild

Requires Python 3.10 or later.

```sh
python3 -m venv .venv
source .venv/bin/activate
python3 -m pip install -r requirements.txt
python3 build.py
```

On Windows, activate the environment with `.venv\Scripts\activate`.

Edit `rankings.json` to change team names, scores, row colors, text colors, or logo paths. Then rerun `build.py`. The script uses bundled assets and does not require internet access. It validates that there are 70 teams with consecutive ranks and scores in descending order, then rebuilds all three output formats.

## Assets and attribution

- Actual team logos downloaded from ESPN’s team logo CDN. Each exact source URL and ESPN team identifier is recorded in `rankings.json`. No logos are AI generated. Some logo variants differ from those shown in the reference. Team logos remain the property of their respective owners.
- Oswald font from Google Fonts, by Vernon Adams, Kalapi Gajjar, and Cyreal. Licensed under the SIL Open Font License, included in `assets/OFL.txt`.
- Stadium and turf background drawn procedurally in Python. Team-cell colors sampled from the supplied reference. The original screenshot is not included in the repository or used as a background.

The SVG text is outlined for consistent portable rendering. `rankings.json` is the editable content source.
