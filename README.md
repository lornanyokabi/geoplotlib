geoplotlib is a python toolbox for visualizing geographical data and making maps

# A first example
To produce a dot density map:

```python
data = read_csv('data/bus.csv')
geoplotlib.dot(data)
geoplotlib.show()
```

This will launch the geoplotlib window and plot the points on OpenStreetMap tiles, also allowing zooming and panning. geoplotlib automatically handles the data loading, the map projection, downloading the map tiles and the graphics rendering with OpenGL.

![demo](http://i.imgur.com/hr9GnLE.gif)

# Examples gallery

[Dot Density Map](https://github.com/andrea-cuttone/geoplotlib/blob/master/examples/dot.py)
![dot](https://raw.githubusercontent.com/andrea-cuttone/geoplotlib/master/examples/screenshots/dotdensity.png)

[Heatmap (Kernel Density estimation)](https://github.com/andrea-cuttone/geoplotlib/blob/master/examples/kde.py)
![kde](https://raw.githubusercontent.com/andrea-cuttone/geoplotlib/master/examples/screenshots/kde1.png)

[Shapefiles](https://github.com/andrea-cuttone/geoplotlib/blob/master/examples/shapefiles.py)
![shapefiles](https://raw.githubusercontent.com/andrea-cuttone/geoplotlib/master/examples/screenshots/shapefiles.png)

[Choroplet and GeoJSON](https://github.com/andrea-cuttone/geoplotlib/blob/master/examples/choroplet.py)
![choroplet](https://raw.githubusercontent.com/andrea-cuttone/geoplotlib/master/examples/screenshots/choroplet.png)

[Voronoi tessellation](https://github.com/andrea-cuttone/geoplotlib/blob/master/examples/voronoi-filled.py)
![voronoi](https://raw.githubusercontent.com/andrea-cuttone/geoplotlib/master/examples/screenshots/voronoi-filled.png)

[Spatial graph](https://github.com/andrea-cuttone/geoplotlib/blob/master/examples/graph-flights.py)
![graph](https://raw.githubusercontent.com/andrea-cuttone/geoplotlib/master/examples/screenshots/graph-flights.png)

All examples including source code are [here](https://github.com/andrea-cuttone/geoplotlib/tree/master/examples)

# Installation

geoplotlib requires:
* [numpy](http://www.numpy.org/)
* [pyglet](http://www.pyglet.org/)
	* **note:** in order for pyglet to work with ipython on Mac, [this workaround](https://code.google.com/p/pyglet/issues/detail?id=728) is needed. [Here](https://code.google.com/r/andreacuttone-pyglet-multipleruns/) you can find a fork of the pyglet dev branch with the workaround applied

optional requirements:
* [matplotlib](http://matplotlib.org/) for colormaps
* [scipy](http://www.scipy.org) for some layers
* [pyshp](https://github.com/GeospatialPython/pyshp) for reading .shp files

to install, run:

```python setup.py install```

# User Guide
A detailed user guide can be found in the [wiki](https://github.com/andrea-cuttone/geoplotlib/wiki/User-Guide)
