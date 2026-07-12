# 1954 AMS Topo Map vs. Fields of the World

A side-by-side swipe comparison of a 1954 AMS Series U502 topographic
survey against [Fields of the World](https://fieldsofthe.world/) —
ML-predicted agricultural field boundaries — over the same patch of
Tamil Nadu, India, between Kanchipuram and Tiruvallur.

**Live demo:** https://untld-net.github.io/geoai-failure-mode/swipe_map.html

## What this is

Left panel: the georeferenced 1954 topo sheet (University of Texas
Libraries, public domain scan). Right panel: FTW's 2024 field-boundary
predictions on a terrain basemap. Drag the divider to compare.

Built to explore a specific question: how do you honestly compare a
71-year-old paper survey against a machine-learning prediction, without
either side implying more precision than its source data actually
supports?

## Stack

[MapLibre GL JS](https://maplibre.org/) + [PMTiles](https://github.com/protomaps/PMTiles)
for both layers (raster for AMS, vector for FTW), served as static
files with no backend. No build step — this is plain HTML/JS.

## Data sources

- AMS Series U502, Sheet ND-44-10 — [University of Texas Libraries](https://maps.lib.utexas.edu/)
- Field boundaries — [Fields of the World](https://source.coop/repositories/ftw/global-data), CC-BY, 2024 vintage
