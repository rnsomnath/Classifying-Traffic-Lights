# Classifying-Traffic-Lights

This project was to classify the red, yellow and green traffic lights with maximum accuracy. I used the computer vision
library in Python (OpenCV) to standardize all the images. I converted the images from RGB to HSV color space. I masked the images on
the basis of the Value in HSV space. I cropped the images from the side and top to remove the irrelevant information. I divided this 
modified image into three regions - top, middle and bottom and calculated the average brightness in each region. Depending on the region 
having the maximum brightness, the image was then classified as having red, yellow and green traffic light.

## **Result:** ##

I could achieve 99% accuracy in the test data. Also, I did not classify even one red light as green, which would prove disastrous in
real life scenario.

## Files used in the project:

### **1. Traffic_Light_Classifier.ipynb**

This file has all the relevant functions to execute the project. The notebook goes through step by step process followed in 
the execution of the project along with the final results.

### **2. helpers.py**

This file contains the function which helps in loading the image dataset from a given directory.

### **3. test_functions.py**

This file has all the functions to test the one-hot encoding of the image labels and also to check whether red lights are 
classified as green.

## Further Improvement:

Some images in the dataset have arrows instead of lights. I wanted to develop an algorithm to classify the lights as round or arrowed.
I am open to collaborating with anyone for the same.



