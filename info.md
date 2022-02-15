[![](https://img.shields.io/github/release/neuhausf/hacs-swiss-public-transport-mod/all.svg)](https://github.com/neuhausf/hacs-swiss-public-transport-mod/releases)
[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/custom-components/hacs)

# hacs-swiss-public-transport-mod

Swiss public transport stationboard and extended platform sensor

## Information

Data from meteo swiss official website

The forecast is extracted from the meteo swiss website

Current conditions are from official data files.
  

## Configuration

- Got to HACS
- Search for "hacs-swiss-public-transport-mod"

Add a new sensor to your configuration.yaml:

```YAML
sensor:
  - platform: swiss_public_transport_mod
    name: Schüpfen
    limit: 4
    stationboard:
    - Schüpfen
```

## Privacy 

This integration uses :

https://github.com/agners/swiss-public-transport-card for geolocaliation if you don't set you post code
the changes made in the pull request by @agners: https://github.com/home-assistant/core/pull/30715
and some own code to adapt the visualization.