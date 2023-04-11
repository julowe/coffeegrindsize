# Coffee Grind Size Short Manual 

By [coffeeadastra.com](http://www.coffeeadastra.com)

This is a summarized version of the Coffee Grind Size software manual. 
For more detailed information, please consult the 
[full version here](https://github.com/jgagneastro/coffeegrindsize/blob/22661ebd21831dba4cf32bfc6ba59fe3d49f879c/Help/coffee_grind_size_manual.pdf). 
For a [quick guide on installation go here](https://github.com/jgagneastro/coffeegrindsize/blob/22661ebd21831dba4cf32bfc6ba59fe3d49f879c/Help/coffee_grind_size_installation.pdf).

The Coffee Grind Size software allows you to measure the size distribution of coffee particles coming out of your grinder. 
In order to use it, take a well-lit picture of your coffee grounds, spread on a white background that does not have any patterns on it. 
Include an object with a known size in your picture, such as a quarter. 
It is very important that the white background is as uniform as possible, and that your coffee grounds don’t create visible shadows on the picture. 
Even more importantly, your coffee grounds should not be touching each other, so do not put too many of them in the picture. 
Try to pour them on a white sheet, and then separate them with either a chopstick or your fingers. 
A decent picture is included in this summary, and a few more are included in the full manual.

The user interface of the Coffee Grind Size software has a toolbar at the top of the window,
with buttons that are organized in a way that you will normally need to use them from left to right. 
Also notice that the software has a status bar at the bottom of the window; pay close attention to it, 
as it will guide you around and tell you if any problem happened.

You will first open an image from your computer (in .PNG or .JPG formats). 
Then you will need to draw a red line to measure the size of your reference object in pixels (don’t include its shadow). 
You will then need to tell the software which reference object you used (either with a dropdown menu, 
or by writing down the actual size of your object in millimetres, with the left-side menu). 
This will allow the software to measure your coffee grounds in real units, rather than pixels.

The next step is to select a region that you would like to analyze with the software. 
You will do this by clicking on the image with the mouse to draw a polygon that includes your coffee grounds, 
but excludes any shadow, light glare, or anything that is not coffee.

Once you are done, click on the “Threshold Image” button. 
This should mark all the coffee grounds in red. 
The software uses the contrast between the dark coffee grounds and the white background to achieve this.

The next step is to click on “Launch Particle Detection”. 
The software will now split all of the pixels in red in distinct particles of coffee. 
It will then show you the distinct coffee particles with an image of their outlines. 
This is a good moment to check that your coffee grounds are not so packed that the software mistakes several particles for one big particle. 
This step is slow !

Then you just need to press “Create Histogram”, and the software will show you a distribution of your coffee particle sizes! 
Please see the full manual for a detailed discussion of all figures you can create, and how you can save, load, 
and compare data from two different pictures. 
Note that the software will be unable to detect the particles smaller than a few pixels!

## Example Images and GUI Info

There are very few clumps of coffee particles in this picture, which is good. 
The upper shadow will still need to be avoided, and there are not that many coffee particles, 
but this is better than an image full of clumps.
![Example of good source picture of adequately spread out coffee grounds on white paper](manual-summarized-1-better-example-picture.jpg)

An example of how a reference object is measured in the software. 
This measurement correctly avoids the coin thickness (lower left side of the image) and the shadows, 
and is taken along the axis perpendicular to the point of view’s inclination. 
This allows the user to obtain an accurate estimate of the size of pixels in their picture.
![image of US quarter with red line from one edge to other, through the center of circle](manual-summarized-2-ref-object.jpg)

![screenshot of application GUI with notes](manual-summarized-3-gui.jpg)

A distribution of the particle surfaces. 
This is an example of what the software can generate for you.
![image of histogram of results from application](manual-summarized-4-histogram.jpg)
