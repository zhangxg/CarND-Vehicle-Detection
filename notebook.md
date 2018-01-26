the object detection: 
1. what is it?
2. where is it? 
3. what is it doing? 

this information can help make a decision of the vehicle. 
this information includes: 
1. the location, 
2. the direction,
3. the speed, 
4. object detection and tracking.  
https://www.quora.com/What-is-the-difference-between-object-detection-and-object-trackin://www.quora.com/What-is-the-difference-between-object-detection-and-object-tracking

---
the template method, why are they not so useful in vehicle detection? 
how to implement a template match method, leave alone theie usefulness;
1. calculate the distance between each pixel. 
2. all methods for similiarity can be used to. 

image histogram

explore the color space, try make drawing on 3d plots;

the HOG feature
https://en.wikipedia.org/wiki/Histogram_of_oriented_gradient://en.wikipedia.org/wiki/Histogram_of_oriented_gradients

https://www.learnopencv.com/histogram-of-oriented-gradients://www.learnopencv.com/histogram-of-oriented-gradients/

opencv and hog; 
opencv and scikit-image, what's their relationship, do they overlap or complement in funcions? 

svm and basic machien learning concepts, such as 3-fold validation etc. 
the scikit-learn package;
in the coursera machine learning course, we are using the graphlib-create package, can be migrated to scikit-learn? 

the sliding window search of the images
the sliding window is less effcient, there are other methods to make the regin proposal. 
the hog sub-sampling window search methods

processing the multiple detection and false postive
the technique is named as head map;

---- the pipeline for the object and tracking
it's all started with the feature extraction, besides the color, this lecture introduced a hog feature, we can combine all these feature together to represt the image;
once we got the feature, now we need to train a classifier, svm is one choice. (yes, in the project i used svm, but definitely can try the deep learning approach)

next, to detec the car in the imagse, we implement a sliding window on the images to draw boxes on the detected area. 
and we may end to that multiple boxes also some false positive, we need to filter them out. 
one appoach is using the heatmap mechanism.

once get the image, we can integrate the work into video processing. 

--------------------
now, we detected the car, to support self driving, we need to know the size and position of the detected objects, or even their speed, how vision provide this informaiton. what's your thought? 

to decide the side distance, i can warp the image, and like the lane line detection part, mapping the pixel to real world; 
for distance to the leading vehicle, i can use the image depth information,   

--------------------
understand what can be done by libraries, and what need to develop. 
the common, difference between libs. 

--------------------
integrate the three project togher, as cv experiment. 

make a presentation of these three. 

