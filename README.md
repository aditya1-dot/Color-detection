# Color-detection
This repository contains Python code for real-time color detection using OpenCV. The code captures video from your webcam and detects three primary colors: red, green, and blue. When any of these colors are detected, rectangles are drawn around them, and their corresponding labels are displayed on the video feed in real-time.

**Prerequisites**

Before running the code, ensure you have the following libraries installed:

-OpenCV (cv2)

-NumPy (numpy)

You can install these libraries using the following command:


```console
pip install opencv-python numpy

```
**How To Use**

-Clone or download this repository to your local machine.

-Open the Python script containing the color detection code.

-Make sure your webcam is connected and accessible.

-Run the Python script.

-The webcam will open, and you will see the live video feed with color detection.

-The code detects red, green, and blue colors and draws rectangles around objects of those colors.

-To exit the program, press the 'q' key.

**Code Explanation**

-The code works as follows:

-It captures video from the webcam using OpenCV.

-It converts each frame of the video from the BGR color space to the HSV color space.

-It defines color ranges for red, green, and blue in the HSV color space and creates masks for each color.

-Morphological transformations (dilation) are applied to the masks to improve color detection.

-Contours are detected in each mask to identify regions of the specified colors.

-If the area of a detected contour is larger than a threshold (300), a bounding rectangle is drawn around it, and a label is displayed.

-The program continuously displays the video feed with real-time color detection until you press the 'q' key, at which point it terminates.

**Troubleshooting**

-If the code is not detecting colors correctly, you may need to adjust the lower and upper HSV range values for each color. Experiment with different values to achieve better color detection.

-Ensure that your webcam is connected and accessible by the code.

-Make sure you have the required libraries installed, as mentioned in the "Prerequisites" section.

Enjoy experimenting with real-time color detection!




