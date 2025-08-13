# Traffic Lights Route

This repository contains a simple Jupyter notebook that plans routes using open data and visualises traffic lights along the way. It relies entirely on OpenStreetMap services so that everything can be run without proprietary map providers.

## Features

- Enter start and end addresses in a notebook interface.
- Geocoding is performed with [OpenStreetMap Nominatim](https://nominatim.openstreetmap.org/).
- Routing is retrieved from the public [OSRM](http://project-osrm.org/) API.
- Traffic lights are loaded from a local GPX or GeoJSON file and displayed on the map.

## Usage

1. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. Add your traffic light file to the `data` folder and name it `traffic_lights.geojson` or `traffic_lights.gpx`.

3. Launch Jupyter and open the notebook:

   ```bash
   jupyter notebook notebooks/traffic_lights_route.ipynb
   ```

4. Type the start and destination addresses in the provided boxes and click **Show Route** to display the map with the route and traffic light markers.

An example GeoJSON file is provided in `data/traffic_lights_sample.geojson` for testing.
