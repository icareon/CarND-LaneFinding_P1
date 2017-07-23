# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps: 

1. Conversion of the image to Grayscale
2. Applying a Gaussian smoothing filter
3. Applying Canny Edge Detection
4. Defining the Region of Interest
5. Applying the Hough Transform
6. Separated the identified lines into left and right lines by the section of the frame they fall in i.e. x> or < 500
7. lumping all x and y values for left and right lines together
8. creating first order polynomial fit to find the linear function that defines the lines
9. redraw the lines based on min and max points in the point list to get full lines


If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
