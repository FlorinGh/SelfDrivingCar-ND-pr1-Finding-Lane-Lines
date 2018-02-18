# **Finding Lane Lines on the Road** 

The goals of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report

---

## Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 6 steps:
- converted the images to grayscale  
- then I apply gaussian blur to remove noise in the image  
- use canny function to detect all edges  
- apply a mask function to elimated edges outside an interest zone  
- use hough function to identify lines  
- draw the identified lines back on the original image to visualy check for acuracy  


### 2. Identify potential shortcomings with your current pipeline

One shortcoming in my pipeline is that it is not robust enough: the parameters used this pipeline are not general enough so that the pipeline can solve any image/movie; a lot manual work is needed to tune these.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to use an algorithm that automaticaly chooses the best parameters.
