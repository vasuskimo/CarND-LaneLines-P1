# **Finding Lane Lines on the Road** 

---

### Reflections

I did not imagine that the process of lane detection would be simple and the process sort of tries to abstract what our eyes would do.
We would look for white lines and our attention would be in a narrow region of the road etc.,

### 1. Description of the pipeline. 

The pipeline comprises of the following:
1.First the image is converted into grayscale.
2.Then a gaussian smoothening is applied.
3. Then the Canny Edge Detection Algorithm is applied.
4. Then the region of interest mask is applied.
5. Then the Hough Transform is applied to identify lane lines.


This resulted in the following:
![https://raw.githubusercontent.com/vasuskimo/CarND-LaneLines-P1/master/test_images/whiteCarLaneSwitch_after.jpg]
![https://raw.githubusercontent.com/vasuskimo/CarND-LaneLines-P1/master/test_images/solidYellowLeft_after.jpg]
![ https://raw.githubusercontent.com/vasuskimo/CarND-LaneLines-P1/master/test_images/solidYellowCurve_after.jpg]
![https://raw.githubusercontent.com/vasuskimo/CarND-LaneLines-P1/master/test_images/test_images/solidYellowCurve2_after.jpg]
![https://raw.githubusercontent.com/vasuskimo/CarND-LaneLines-P1/master/test_images/test_images/solidWhiteRight_after.jpg]
![https://raw.githubusercontent.com/vasuskimo/CarND-LaneLines-P1/master/test_images/test_images/solidWhiteCurve_after.jpg]


### 2. Potential shortcomings with the current pipeline


One shortcoming would be when the road winds a lot, my code would not be able to handle well.
The other obvious shortcoming is, when the light suddenly changes, my code needs to handle.


### 3. Possible improvements to the current pipeline

A possible improvement would be to use different shapes for the region of interest, play more with the tuning parameters. 
