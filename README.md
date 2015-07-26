MORPS - Modifying Objects to Reduce Python Scripting
========

Python should be simple. Writing ~50 lines of code to create one buffer is not simple. 

Morps attempts to simplify geoprocessing with Python. Using the terminal/command line interface, navigate to the directory storing the morps.py file. 

Type 
    
    python 

as the command and begin using morps:

    import morps

    cities = "data/cities.shp"
	cities_buffered = "data/cities_buffered.shp"
	unit = 'miles'
	format = 'shp'

	morps.buffer(cities,cities_buffered,500,unit,format)

or even simpler:

	morps.buffer("data/cities.shp","data/cities_buffered.shp","miles","shp")


This library is built on top of GDAL, and is required to be installed in order for MORPS to work correctly. Find GDAL install instructions here- https://www.mapbox.com/tilemill/docs/guides/gdal/

If you do not get errors when typing <b>import ogr</b> into Python, you know that Python is configured and you are ready to use morps.

The code in this repo is also intended to demonstrate how one could utilize the OGR vector library within GDAL 
for performing basic geoprocessing tasks.


Other useful online resources for GDAL:

<ul>
<li>Geoprocessing with Python using Open Source GIS- http://www.gis.usu.edu/~chrisg/python/2009/</li>
<li>GDAL Homepage- http://www.gdal.org/index.html</li>
<li>OGR Classlist- http://www.gdal.org/ogr/annotated.html</li>
<li>OGR Hierarchy, super useful for understanding geometry features- http://www.gdal.org/ogr/hierarchy.html</li>
<li>OGR2OGR Cheatsheet- http://www.bostongis.com/PrinterFriendly.aspx?content_name=ogr_cheatsheet</li>
<li>Converting spatial data using OGR2OGR- http://giscollective.org/#/spatial-data-conversion-using-python/</li>
</ul>
