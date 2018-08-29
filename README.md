# MaxPlot: A library for fast scatter plots

MaxPlot is like many other scatter plot libraries: you can give it a div, give it coordinates
and colors and it will plot little circles.

One difference is that this one will plot up to 1 million circles and without using WebGL.

It comes with a basic navigation UI: three different modes (zoom, select, move), +/- zoom and 100% zoom.

It can call javascript functions with the IDs of the circles when the user
selects or hover over the circles.

It's really easy to use:

    document.body.appendChild(div);
    var fig = new MaxPlot(div, 50, 50, 800, 400, {'radius':30, 'alpha':1.0});
    fig.initPlot({'radius':30, 'alpha':0.8});
    // set the coordinates
    fig.setCoords([1,2, 2,3, 3,4, 4,5, 2.02, 3.02], [[2.5,2.5, "a label"], [1.5,1.5, "the green circle covers another circle. Zoom onto it."]]);
    // set four different colors
    fig.setColors(["000000", "ff0000", "00ff00", "0000ff"]);
    // and assign every circle its color
    fig.setColorArr([0, 1, 2, 3, 2]);
    // and draw the plot
    fig.drawDots();

Look at index.html for an example how to use it.

You can also play with the example <a href="http://hgwdev.soe.ucsc.edu/~max/maxPlot/">here</a>.
