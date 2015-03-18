geopandas_osm
======

A GeoPandas interface to query OpenStreetMap Overpass API
   
Quick start
-------------------------

.. code-block:: python

    import geopandas_osm.osm
    df = geopandas_osm.osm.query_osm('way', poly.bounds, recurse='down', tags='highway')
    


Project skeleton based on http://github.com/mapbox/pyskel
