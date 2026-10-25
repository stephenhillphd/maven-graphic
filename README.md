# Maven Graphic: College Football Résumé Rankings

A code recreation of a college football résumé rankings graphic, with real team logo assets. All 70 teams, rankings, and scores are transcribed from the reference image, including ties and Northern Illinois at -0.36. These are reference scores, not live ratings.

## Files

- `output/college-football-rankings.html`: standalone browser version of the graphic
- `reference/reference-rankings.webp`: the original reference image the graphic was transcribed from

## View the graphic

Download or clone the repository and open `output/college-football-rankings.html` in a modern browser. The HTML is a single self-contained file and works offline. It includes PNG and SVG download buttons and a drawer with the editable ranking data as JSON.

The build script, `rankings.json`, and the source assets used to generate the HTML are not in this repository. The JSON in the drawer can be downloaded, but rebuilding the graphic from it requires those files.

## Assets and attribution

- Team logos come from ESPN's team logo CDN. Some logo variants differ from those shown in the reference. Team logos remain the property of their respective owners.
- The reference image is included for comparison only and is not used as a background in the HTML.
