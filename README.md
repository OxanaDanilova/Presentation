# Transcript of the Presentation

Hello everybody. I am Oksana and I'm going to say about HTML canvas element
00:10
so what is HTML canvas? - canvas element is used to draw graphics on the fly via scripting. it's only a container for the graphics and we must use 
JavaScript to actually draw the graphics
00:31
as I said before - Canvas element is used to draw graphics on the web page. On this slide we can see some graphic elements which were created with a
canvas element. We can see red rectangle, gradient rectangle, multicolor rectangle and multicolored text.
01:06
So what can we draw? With this canvas we can draw text
01:11
We can draw graphics. It can be animated, can be interactive and of course, it can be used in games. 
01:28
so how to start?
First of all you must find the canvas element.
01:33
 This is done by using get element by ID Dom method. Secondly you must create a drawing object
01:54
The getContext() is a built-in HTML object, with properties and methods for drawing:
02:08
And finally we can specify color for the graphics and draw something on the canvas. 
02:26
In order to specify color we can use fill style property and here we can
specify CSS color, gradient or pattern
02:36
and then we can draw some object. 
02:41
For example I want to draw red rectangle. 
02:46
For this goal I use fillRect method
02:49
where X Y coordinates of left top corner
02:55
of this rectangle and width, height - width
03:01
and height of this rectangle. 
03:10
HTML canvas coordinates. HTML canvas coordinates is
2 dimensional grid and top left
03:23
corner of this grid has a coordinate (0,0). 
03:28
The origin can be moved and
03:32
translate with translate() function, where
03:37
positive numbers define amount of pixels
03:44
to move right and down.
03:53
Geometric primitives 
03:55
Geometric primitives are simplest
04:02
shapes which can be drawn with canvas
04:09
element. It could be line,
04:11
rectangle, triangle, ellipse, arrow, star
04:17
How to draw a line? For this goal I can
04:22
use moveTo() method with X Y parameters
04:30
Here we define starting point of this
04:35
line, then we can use lineTo() method
04:40
with x1 y1 parameters, where we can
04:45
specify ending point of this line and in
04:53
order to actually draw this line we must
04:57
use stroke() method 
05:03
How to draw a circle?
For this goal we can use the beginPath()
05:08
method and then arc method with X Y
05:15
radius, startangle and endangle parameters,
05:18
where X Y - coordinates of the center of
05:23
this circle, radius - radius of this circle
05:28
and startangle and endangle. 
05:39
In order to actually draw this circle we
05:42
can use stroke() method 
05:54
Canvas gradients
Some graphics elements such as lines,
05:58
rectangle, circle and also some text can
06:04
be filled by gradients. There are two
06:08
types of gradients: linear gradient and
06:12
radial gradient. In order to
06:15
create some gradients we must use createLinearGradient(x,y,x1,y1) or createRadialGradient(x,y,r,x1,y1,r1)
06:22
and also we can add two or
06:28
more colors in this gradient and specify
06:34
position of this color in gradient. We can
06:38
make it with addColorStop() method.
06:45
On this slide we can see some examples of
06:49
linear gradient and radial gradient
06:58
Of course we can draw text on the HTML
07:03
canvas element. For this goal we can use
07:10
some important property and methods - such
07:13
as font, which defines font of the text
07:18
and also fillText(text,x,y) and strokeText(text,x,y)
07:23
method. On this slide we can use some
07:30
examples of fillText() and strokeText()
07:34
method. Here we create filled text 
07:40
 and here we can create non-filled
07:47
text. And also we can specify color of
07:54
this text and put text in the center of
07:59
the canvas area.
08:06
Animation. Animation is moving object
08:11
from one position to another and making
08:17
this process smooth. And in order to
08:28
create animation first of all we can
08:33
draw the object which we want to animate.
08:38
For example I create circle. And secondly
08:46
in order to create animation we can use
08:50
requestAnimationFrame. So here I create
08:55
function animate and increase X Y
09:04
parameters - X Y coordinates of the center
09:11
of the circle. It looks good, but could be
09:18
better. And finally we can use ClearRect()
09:24
method in order to update and 
09:30
clear canvas area between animation
09:36
frames. So I specify this method here and
09:43
in this method i specify X Y parameters
09:52
of this area and width hight parameters of
10:00
this area's rectangle and now it should
10:12
look better 
10:17
Of course animation could be used in games. For these goals
10:21
we must add some couples of event
10:28
listeners and for example mouse click
10:34
mouse move 
10:41
and so on and handle this event with
10:47
JavaScript. So this actually all what I
10:52
want to say for this topic.
10:54
Thank you for your attention. Goodbye.