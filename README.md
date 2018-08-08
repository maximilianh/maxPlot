# MaxPlot: A library for fast scatter plots

MaxPlot is like many other scatter plot libraries: you can give it a div, give it coordinates
and colors and it will plot little circles.

One difference is that this one will plot up to 1 million circles and without using WebGL.

It comes with a basic navigation UI: three different modes (zoom, select, move), +/- zoom and 100% zoom.

It can call javascript functions with the IDs of the circles when the user
selects or hover over the circles.

Look at index.html for an example how to use it.

You can also play with the example <a href="http://hgwdev.soe.ucsc.edu/~max/maxPlot/">here</a>.
