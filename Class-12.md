A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

Setting up:
The first thing we need to do is download directly from here: (Chart.js)[https://registry.npmjs.org/chart.js/-/chart.js-3.3.2.tgz] Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script Chart.min.js

to prepare for Charts we need to add canvas element to the body of HTML:

example: <canvas id="buyers" width="600" height="400"></canvas>

and we need also to write a script that will retrieve the context of the canvas, so add as example this to the foot of your body element:

<script> var buyers = document.getElementById('buyers').getContext('2d'); new Chart(buyers).Line(buyerData); </script>

Drawing a line chart:
Inside the same script tags we need to create our data, in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart. Add this immediately above the line that begins ‘var buyers=’:

var buyerData = { labels : ["January","February","March","April","May","June"], datasets : [ { fillColor : "rgba(172,194,132,0.4)", strokeColor : "#ACC26D", pointColor : "#fff", pointStrokeColor : "#9DB86D", data : [203,156,99,251,305,247] } ] }

Drawing a bar Chart:
same process of creating line chart but instead of use .line like here: new Chart(buyers).Line(buyerData); we use .Bar with name of variables for Bar Chart. and fill the data to draw.

Drawing Pie Chart:
This will be easier, first use .Pie in new Chart instead of .Line as in Line Chart… and the data will be simple just contain value and color.

Sample of Charts

Canvas API
Basic usage of canvas:
The <canvas> element:
<canvas> element has only two attributes, width and height. These are both optional.

if you didn’t set them, canvas will initially be 300 pixels wide and 150 pixels high

The element can be sized by CSS but must respect atio of the initial canvas.

The <canvas> element creates a fixed-size drawing surface that exposes one or more rendering contexts getContext() used to obtain the rendering context and its drawing functions. it takes one parameter, the type of context. For 2D graphics
