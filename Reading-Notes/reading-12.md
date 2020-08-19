# Chart.js, Canvas
<br>

Online Article on [Animated Charts](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)
<br>

### Charts

Charts are better for displaying data visually than tables. A great way to get started on using charts is with the chart.js plugin. follow the link above to download. Then slam this in the head:
<br>

!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8" />
        <title>Chart.js demo</title>
        <script src='Chart.min.js'></script>
    </head>
    <body>
    </body>
</html>
<br>

Now you can draw line, pie, and bar charts for data using specific colors. The exact syntax for each is also provided on the website. 
<br>

### Canvas
<br>

The tag <canvas> is like an image tag but but for <video>, <audio>, or <pictures>. It is easy to design some fallback content incase your browser doesnt load with this tag. Example of a canvas tag:
<br>

<canvas id="clock" width="150" height="150">
  <img src="images/clock.png" width="150" height="150" alt="clock"/>
</canvas>
<br>

or
<br>

<canvas id="stockGraph" width="150" height="150">
  current stock price: $3.15 + 0.15 
</canvas>
<br>

The canvas element creates a fixed-size drawing surface that exposes one or more **rendering contexts**. Canvas only supports two primitive shapes: rectanges and paths (lists of points connected by lines.) All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes. Ex.
<br>

function draw() {
  var canvas + document.getElementById('canvas')
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.fillRect(25,25,100,100);
    ctx.clearRecct(45,45,60,60);
    ctx.strokeRect(50,50,50,50);
  }
}
<br>

You can draw all sorts of shapes using lines and filling them with canvas. You can get creative and make some very interesting patterns. Using bezierCurveTo(x,y,z,a,b,c) you can create multi angles shapes like a heart. There is an example here that allows you to make an entire pac man game dashboard, complete with pac man and a ghost. You can mess with just about anything, the possibilities dont end there, you can add colors and manipulate text aswell. All links to these styles are in your code file on google chrome, under canvas.


[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)