# **Finding Lane Lines on the Road** 
<img src="examples/laneLines_thirdPass.jpg" width="480" alt="Combined Image" />

Overview
---

My pipeline consisted of:
1. Converting the image to grayscale to make it easier to run computations on the pixels
2. Using GAussian Blur as some kind of low pass filter to remove high frequency pixels and make all pixels more like their neighboring pixel and smoothen out the edges
3. Use Canny edge detection to find all the edges in the image.
4. Use a mask to cover parts of the image not considered to be lane lines
5. Use Hough lines to represent the lane lines mathematically

