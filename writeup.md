# **Finding Lane Lines on the Road** 

[//]: # (Image References)

[image1]: ./test_images/whiteCarLaneSwitch_after.jpg 
[image2]: ./test_images/solidYellowLeft_after.jpg
[image3]: ./test_images/solidYellowCurve_after.jpg
[image1]: ./test_images/solidYellowCurve2_after.jpg
[image1]: ./test_images/solidWhiteRight_after.jpg
[image1]: ./test_images/solidWhiteCurve_after.jpg
---

### Reflection

I did not imagine that the process of lane detection would be simple and the process sort of tries to abstract what our eyes would do.

We would look be focused on white lines and our attention would be in a narrow region of the road etc.,

### 1. Description of the pipeline. 

The pipeline comprises of the following:
1.First the image is converted into grayscale.
2.Then a gaussian smoothening is applied.
3. Then the Canny Edge Detection Algorithm is applied.
4. Then the region of interest mask is applied.
5. Then the Hough Transform is applied to identify lane lines.


This resulted in the following:
![alt text][image1]
![alt text][image2]
![alt text][image3]
![alt text][image4]
![alt text][image5]
![alt text][image6]


### 2. Identify potential shortcomings with your current pipeline


One shortcoming would be when the road winds a lot,my pipeline would not handle.
The other obvious shortcoming is, when the light suddenly changes, my code needs to handle.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to use different shapes for the region of interest, play more with the tuning parameters. 

Another potential improvement could be to ...
