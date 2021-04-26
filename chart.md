# CHARTS

*Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.*

1. Setting up :
    * create a new html page and import the script: <br> 
    \<script src='Chart.min.js'>\</script>
2. Drawing a line chart:
    *  create a canvas element in our HTML: <br> 
    \<canvas id="buyers" width="600" height="400">\</canvas>
    * write a script that will retrieve the context of the canvas:
    <br> \<script> <br>
    var buyers = document.getElementById('buyers').getContext('2d');<br>
    new Chart(buyers).Line(buyerData); <br>
    \</script> <br>
    * Inside the same script tags we need to create our data

    * ![line](https://apexcharts.com/wp-content/uploads/2018/01/basic-line-chart.svg)
3. Drawing a pie chart:
    * ![pie](https://www.js-tutorials.com/wp-content/uploads/2016/08/pie-chart-using-chatrsjs-1200x675.png)
4. Drawing a bar chart:
    * ![bar](https://miro.medium.com/max/2908/1*s9ACgOrgGMCCwQKf-p88sQ.png)

<br>
<br>

### Drawing shapes with canvas
1. Drawing rectangles
    * fillRect(x, y, width, height) :Draws a filled rectangle.
    * strokeRect(x, y, width, height): Draws a rectangular outline.
    * clearRect(x, y, width, height): Clears the specified rectangular area, making it fully transparent.
2. Drawing paths:
    * beginPath() :
    Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
    * closePath():
    Adds a straight line to the path, going to the start of the current sub-path.
    * stroke():
    Draws the shape by stroking its outline.
    * fill(): 
    Draws a solid shape by filling the path's content area.
3. Drawing a triangle.

<br>'
<br>
### Applying styles and colors
1. fillStyle = color
    * Sets the style used when filling shapes.
2. strokeStyle = color
    * Sets the style for shapes' outlines.
    <br>
    <br>

### Drawing text
*The canvas rendering context provides two methods to render text:*

1. fillText(text, x, y [, maxWidth])
    * Fills a given text at the given (x,y) position. Optionally with a  maximum width to draw.
2. strokeText(text, x, y [, maxWidth])
    * Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.



