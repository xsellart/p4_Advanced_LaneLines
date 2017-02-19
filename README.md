# p4_Advanced_LaneLines

##By Xavier Sellart

##Overview

The goals / steps of this project are the following:
 * Compute the camera calibration matrix and distortion coefficients given a set of chessboard images.
 * Use color transforms, gradients, etc., to create a thresholded binary image.
 * Apply a distortion correction to raw images.
 * Use color transforms, gradients, etc., to create a thresholded binary image.
 * Apply a perspective transform to rectify binary image ("birds-eye view").
 * Detect lane pixels and fit to find the lane boundary.
 * Determine the curvature of the lane and vehicle position with respect to center.
 * Warp the detected lane boundaries back onto the original image.
 * Output visual display of the lane
 
##Files structure
The project files are organized as follows:
 * _camera_cal_: Folder containing the chessboards images for camera calibration
 * _output_images_: Folder containing the results of the implemented algorithms.
 * _test_images_: Folder containing the images used for testing the algorithms.
 * _p4_Advanced_Lane_Lines.ipynb_: Jupyter notebook where the algorithms are executed and the results displayed.
 * _project_video.mp4_: It's the video which used to test the performance of the pipeline.
 * _white.mp4_: It's the result of executing the pipeline in the project_video.mp4
 * _writeup_XavierSellart_: It's a document explaining all the algorithms.

##Conclusions
The most difficult part of the project has been to detect the lanes from the binary image because it was quite challenging to find the right way of making windows which where filtering each frame of the video and also to find the correct decisions for deciding if the detected lanes were wrong or fine.
However, the part which has to be improved to make this system work in all the situations in the real world is the part of generating the binary image. It’s quite important to make this algorithm work under any circumstances in the real world and this will complicate a lot the work for tuning the correct parameters or finding the best techniques to get the correct binary data.

Furthermore, if this has to be implemented in real-time it will be also necessary to optimize the code in order to meet the real-time requirements.
It has been amazing to learn how to use Open CV functions and python libraries in order to do these kind of algorithms. I’m quite surprised in how much you can do with these tools.
