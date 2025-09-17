# quakelib notes

## data formats

- [GeoJSON](https://geojson.org/)
  - [geojson Python package](https://pypi.org/project/geojson/)
  - [USGS: GeoJSON summary](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php)
  - [USGS: GeoJSON detail](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson_detail.php)
- [QuakeML 2.0](https://quake.ethz.ch/quakeml/QuakeML2.0)
  - [USGS: QuakeML summary](https://earthquake.usgs.gov/earthquakes/feed/v1.0/quakeml.php)

## web services

- [FDSN](https://www.fdsn.org/webservices/)
- [SeismicPortal](https://www.seismicportal.eu/webservices.html)

## earthquake data providers

### modern

- [USGS](https://earthquake.usgs.gov/earthquakes/feed/)
- [EMSC](https://www.emsc-csem.org/Earthquake_data/Data_queries.php)
- [GEOFON](https://geofon.gfz-potsdam.de/eqinfo/)
- [Kövesligethy Radó SZO](http://www.seismology.hu/index.php/hu/)

### historical

- [AHEAD - European Archive of Historical EArthquake Data](https://www.emidius.eu/AHEAD/index.php)
- [GHEA - Global Historical Earthquake Archive](https://emidius.eu/GEH/)

## data acquisition

### historical

#### AHEAD

- data: event parameters
- standard: [FDSN (fdsnws-event)](https://www.emidius.eu/AHEAD/services/events.php)
- base url: `https://www.emidius.eu/fdsnws/event/1/`
  - `query?`
    - `param1=xxx&param2=xxx&...`
    - `eventid=xxx`
  - or `https://www.emidius.eu/fdsnws/event/1/id/xxxx`
- output: GeoJSON, QuakeML
