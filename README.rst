geopandas_osm
======

A GeoPandas interface to query OpenStreetMap Overpass API
   
Customization quick start
-------------------------

To use pyskel as the start of a new project, do the following, preferably in
a virtual environment. Clone the repo.

.. code-block:: python

    import geopandas_osm.osm
    df = geopandas_osm.osm.query_osm('way', poly.bounds, recurse='down', tags='highway')
    

