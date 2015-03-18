geopandas_osm
======

A GeoPandas interface to query OpenStreetMap Overpass API
   
Quick start
-------------------------

Assuming you have a polygon for a boundary

.. code-block:: python

    import json
    
    import shapely.geometry
    import geopandas_osm.osm
    
    with open('boundary.geojson') as f:
        data = json.load(f)
        
    poly = shapely.geometry.shape(data['features'][0]['geometry'])
    df = geopandas_osm.osm.query_osm('way', poly, recurse='down', tags='highway')
    


Project skeleton based on http://github.com/mapbox/pyskel
