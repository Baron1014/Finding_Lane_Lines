## Finding lane lines of highway
The Self-Driving Car System for Lane Detection on Highways is a project that aims to develop a reliable lane detection system for autonomous vehicles. Lane detection is a crucial component of self-driving cars, as it helps them navigate safely on the road. This system uses image processing techniques to detect and identify the lane lines on the road.

The first step of the system is color selection. Since the lane lines are typically white or yellow, the system uses color filtering to isolate these relevant portions of the image. The next step is to mask the region of interest, which is a trapezoidal area in the center of the image that corresponds to the road ahead. This step helps to filter out any irrelevant parts of the image and discard any pixels outside of the region of interest.

The color and region selection steps are then combined to create a binary image. This binary image is passed through a Canny edge detection algorithm, which detects edges in the image. This step helps to identify the lane lines as edges in the image. Before performing the Hough Transform, a Gaussian blur is applied to the Canny edges image. This step helps to remove any noise and smoothes out the edges, which results in more accurate lane detection.

Finally, the Hough transform is applied to the smoothed Canny edges image to detect the straight lines that correspond to the lane markings on the road. The Hough transform is a mathematical technique that can identify lines in an image based on their parameters, such as slope and intercept.

### Youtube Video result
[![Taiwan_Highway](https://img.youtube.com/vi/kfNl_zSDx68/maxresdefault.jpg)](https://www.youtube.com/watch?v=kfNl_zSDx68)
