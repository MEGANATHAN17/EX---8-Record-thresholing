# EX---8-Record-thresholing

# Aim
To segment an image using Global Thresholding, Adaptive Thresholding, and Otsu's Thresholding techniques using Python and OpenCV.

The program performs the following operations:

Global Thresholding
Adaptive Thresholding
Otsu's Thresholding
Software Used
Anaconda – Python 3.7
Jupyter Notebook / VS Code
OpenCV (cv2)
NumPy
Matplotlib

# Algorithm
Step 1:
Import the required libraries: OpenCV, NumPy, and Matplotlib.

Step 2:
Load the input image using OpenCV.

Step 3:
Convert the input image into grayscale format.

Step 4: Global Thresholding
Select a fixed threshold value.
Apply thresholding to separate foreground and background pixels.
Display the thresholded image.

Step 5: Adaptive Thresholding
Compute threshold values for small regions of the image.
Apply Adaptive Mean Thresholding.
Apply Adaptive Gaussian Thresholding.
Display the segmented images.

Step 6: Otsu's Thresholding
Automatically determine the optimal threshold value.
Apply Otsu's thresholding technique.
Display the segmented image.

Step 7:
Compare the results obtained from Global, Adaptive, and Otsu's thresholding methods.


# Developed By

Name: MEGANATHAN R

Register No: 212224230156

# PROGRAM:
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
image = cv2.imread('1.jpg') 
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY) 
plt.subplot(2, 2, 1)
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))  
plt.title("Original Image")
plt.axis('off')
```

# OUTPUT:
<img width="385" height="180" alt="image" src="https://github.com/user-attachments/assets/7d5496c0-69bf-46db-a926-b8cc777af708" />


# PROGRAM:
```
plt.subplot(2, 2, 2)
plt.imshow(global_thresholded, cmap='gray')
plt.title("Global Thresholding")
plt.axis('off')

plt.subplot(2, 2, 3)
plt.imshow(adaptive_thresholded, cmap='gray')
plt.title("Adaptive Thresholding")
plt.axis('off')

plt.subplot(2, 2, 4)
plt.imshow(otsu_thresholded, cmap='gray')
plt.title("Otsu's Method")
plt.axis('off')

plt.tight_layout()
plt.show()
```

# OUTPUT:

<img width="764" height="492" alt="image" src="https://github.com/user-attachments/assets/4c70660a-b608-4664-93a2-8f957bbd0d33" />


# Result

Thus, image segmentation is successfully performed using Global Thresholding, Adaptive Thresholding, and Otsu's Thresholding techniques in OpenCV.

