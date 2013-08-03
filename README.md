paint5
======

paint5 is a simple painting application built on basic Javascript and HTML5 standards.

A simple explanation of how the painting works is as follows:

A javascript function continually keeps track of the position of the cursor inside the canvas element. The canvas
has and 'onMouseMove' event that fires a function to check if the mouse button is down. If the mouse button is down,
then the function calls the 'paint' function which accepts arguments of position (x,y), pen width in pixels, pen width,
pen color, and a reference to which canvas is to be painted on. It then paints on the canvas until the mouse button is 
released. The color chooser is HTML5's builtin function. I have a function that is fired when the color or pen width is
changed that updates the values that 'paint' uses. Lastly, there is a string at all times in the upper left hand corner
that tells the (x,y) position of the cursor as it moves. 

The clear function is pretty simple, it simply writes over the canvas selected.
The save funtion dumps the canvas to img/png format and prints a link where the reference is a base64 encoded version
of the image.
