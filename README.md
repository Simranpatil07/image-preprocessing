# image-preprocessing

EXP1-A RESIZING
Scaling operations increase or reduce the size of an image. 
When the python image is resized, the interpolation method defines how the new pixels are computed. There are several interpolation techniques, each of which has its own quality vs. speed trade-offs.
It is important to note that resizing an image can reduce its quality. This is because the new pixels are calculated by interpolating between the existing pixels, and this can introduce some blurring.


EXP1-B IMAGE ROTATION
Images can be rotated to any degree clockwise or otherwise. We just need to define rotation matrix listing rotation point, degree of rotation and the scaling factor. 
The rotation angle can be positive or negative. A positive angle rotates the image clockwise, while a negative angle rotates the image counterclockwise.
The scale factor can be used to scale the image up or down. A scale factor of 1 will keep the image the same size, while a scale factor of 2 will double the size of the python image.


EXP1-C IMAGE TRANSLATION
Translating an image means shifting it within a given frame of reference that can be along the x-axis and y-axis.
The translation parameters are specified in the transformation matrix as the tx and ty elements. The tx element specifies the amount of translation in the x-axis, while the ty element specifies the amount of translation in the y-axis.


EXP1-D IMAGE SHEARING
Image shearing is a geometric transformation that skews an image along one or both axes i.e x or y axis.
To shear an image using OpenCV, we need to create a transformation matrix. This matrix is a 2×3 matrix that specifies the amount of shearing in each direction.
The shearing parameters are specified in the transformation matrix as the shearX shearY elements. The shearX element specifies the amount of shearing in the x-axis, while the shearY element specifies the amount of shearing in the y-axis.


EXP1-E NORMALIZE IMAGE
Image normalization is a process of scaling the pixel values in an image to a specific range.This is often done to improve the performance of image processing algorithms, as many algorithms work better when the pixel values are within a certain range.
The normalization type specifies how the pixel values are scaled. There are several different normalization types available, each with its own trade-offs between accuracy and speed.
Image normalization is a common preprocessing step in many image processing tasks. It can help to improve the performance of algorithms such as image classification, object detection, and image segmentation.


EXP1-F IMAGE EDGE DETECTION
The process of image edge detection involves detecting sharp edges in the image. This edge detection is essential in the context of image recognition or object localization/detection. There are several algorithms for detecting edges due to its wide applicability.

In image processing and computer vision applications, Canny Edge Detection is a well-liked edge detection approach. In order to detect edges, the Canny edge detector first smoothes the image to reduce noise, then computes its gradient, and then applies a threshold to the gradient. The multi-stage Canny edge detection method includes the following steps:
Gaussian smoothing: The image is smoothed using a Gaussian filter to remove noise.
Gradient calculation: The gradient of the image is calculated using the Sobel operator.
Non-maximum suppression: Non-maximum suppression is applied to the gradient image to remove spurious edges.
Hysteresis thresholding: Hysteresis thresholding is applied to the gradient image to identify strong and weak edges.
The Canny edge detector is a powerful edge detection algorithm that can produce high-quality edge images. However, it can also be computationally expensive.


EXP1-G  Image Blurring
Image blurring is the technique of reducing the detail of an image by averaging the pixel values in the neighborhood. This can be done to reduce noise, soften edges, or make it harder to identify a picture. In many image processing tasks, image blurring is a common preprocessing step. It is useful in the optimization of algorithms such as image classification, object identification, and image segmentation. In OpenCV, a variety of different blurring methods are available, each with a particular trade-off between blurring strength and speed.
Some of the most common blurring techniques include:
Gaussian blurring: This is a popular blurring technique that uses a Gaussian kernel to smooth out the image.
Median blurring: This blurring technique uses the median of the pixel values in a neighborhood to smooth out the image.
Bilateral blurring: This blurring technique preserves edges while blurring the image.


EXP1-H   Morphological Image Processing
Morphological image processing is a set of python image processing techniques based on the geometry of objects in an image. These procedures are commonly used to eliminate noise, separate objects, and detect edges in images.
Two of the most common morphological operations are:
Dilation: This operation expands the boundaries of objects in an image.
Erosion: This operation shrinks the boundaries of objects in an image.
Morphological procedures are often used in conjunction with other image processing methods like segmentation and edge detection.
