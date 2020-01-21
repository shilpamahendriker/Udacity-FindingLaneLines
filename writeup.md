# **Finding Lane Lines on the Road** 



---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road



[//]: # (Image References)

[image1]: ./test_images_output/solidWhiteCurve.jpg


---

### Reflection



My pipeline starts with converting the images to grayscale, applying Gaussian smoothing module using Canny Edge Detection,selecting the region of interest, applying Hough Tranform line detection and finally combining original image with Hough lines

To make a single line on the left and right lanes, I modified the draw_lines() function first by segregating left and right lines by using slope.Calculated the average of slopes on each side and drew a continuious line representing the lanes.


![alt text][image1]


### Potential shortcomings with your current pipeline

Some of potential shortcomings in this model would be if the lanes are curvy, if there are any other lane markings and if the roads are very reflective the results not be  so accurate.


### Improvements to your pipeline

Converting the image into darker scale to get more clear lane markings and improve the functionality to consider the curvy lanes.
