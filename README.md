# Gradient-Along-Stroke-by-value

This example shows how to create a gradient that follows a stroke by z-value. There are two main techniques for creating a gradient on a line or path in D3; by using gradient units which defined as <a href="https://www.w3.org/TR/SVG/pservers.html#LinearGradientElementGradientUnitsAttribute">userSpaceOnUse</a> (<a href="https://bl.ocks.org/mbostock/3969722">d3 gradient encoding example</a>), or by sampling path uniformly (<a href="https://bl.ocks.org/mbostock/4163057">d3 gradient along stroke example</a>). Somtimes, however, you may have to use z-value to represent the color gradient for each line poisition value.

To start, get the SVG path element and use getPointAtLength. The precesion for sampling is calculated to match the length of the data, and pass the value according to the index value to the initiated color function to create the gradient. 

The code was inspired from <a href="https://bl.ocks.org/mbostock/4163057">d3 gradient along stroke example</a> of <a href="https://bl.ocks.org/mbostock">Mike Bostock</a>
