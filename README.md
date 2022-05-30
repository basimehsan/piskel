Addition of a Soft Brush
One of the additions we proposed in the piskelapp project was the addition of a custom soft brush. The project does have the functionality of painting with a brush(the app calls it a ‘Pen Tool’).

We added to the functionality and now the user can also use a soft brush instead of a default hard edge brush.

Now, let’s get over how we implemented this new functionality into the piskel app. The Pen Tool by default draws on a single pixel on the canvas. We modified the code such that when the user clicks on a pixel using the Pen tool, not only the color is applied on that pixel but a similar color of a lesser intensity is applied on the surrounding pixels as well. The surrounding pixels are applied a color of a lesser intensity to give the user the impression of a soft edge. That is how we implemented a soft edged brush.


Code Walkthrough


What this code does is that not only does it apply color on the pixel being clicked on but also on all the 8 pixels surrounding it. The result can be observed in the following figure:


Now, what we do is that we make the surrounding pixels a lighter shade of the color of the central pixel. It is done as:



Following code is used to convert the given color to a lighter shade of it:




The result is as follows:

Here’s another instance of it in action:



Now, the task is complete.

