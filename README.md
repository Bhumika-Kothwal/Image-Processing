# Image-Processing
## Tables of Contents
  * [About](#about)
  * [Task 1](#task-1)
  * [Task 2](#task-2)
    * [Blurring Image](#blurring-image)
    * [Sharpening Image](#sharpening-image)
  * [Task 3](#task-3) 
  * [Task 4](#task-4)
  * [Task 5](#task-5) 
  * [Task 6](#task-6) 
   
## About
The tasks are performed without using any of the libraries such as cv2 unless specified. The packages used are Numpy and PIL.         
Done under the guidance of SRA VJTI.
## Task 1
### 1. Image Rotation
Rotating the given image by various angles without the use of inbuilt rotate functions of numpy, PIL or OpenCV. The white spaces which were created in the image after rotation were filled by copying the pixeles from the neighbouring cell to the cell containing white space.   
The rotation matrix with explaination can be found [here](https://scipython.com/book/chapter-6-numpy/examples/creating-a-rotation-matrix-in-numpy/
). 

Original image                     |  Rotating it by 50 degree
:-------------------------:|:-------------------------:
<img width="640" height="450" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Image%20Rotation/rotate.png">|<img width="640" height="450" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Image%20Rotation/rotated_50.png">
   
## Task 2
### Blurring Image
Blurring the image with 5x5 kernels without using inbuilt functions. When we blur an image, we make the color transition from one side of an edge in the image to another smooth rather than sudden. The effect is to average out rapid changes in pixel intensity. The blur, or smoothing, of an image removes “outlier” pixels that may be noise in the image. Blurring is an example of applying a low-pass filter to an image. In computer vision, the term “low-pass filter” applies to removing noise from an image while leaving the majority of the image intact. A blur is a very common operation we need to perform before other tasks such as edge detection.    
The explaination and kernels for blurring can be found [here](https://www.tutorialspoint.com/dip/concept_of_blurring.htm
).      
For understanding gaussian blur, [this](https://homepages.inf.ed.ac.uk/rbf/HIPR2/gsmooth.htm
) would be helpful.

 Original image  | Box Blur  | Weighted Average Blur | Gaussian Blur 
:-----:|:-----:|:-----:|:-----:
<img width="240" height="300" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Applying%20Kernels/blur_input.jpeg">|<img width="240" height="300" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Applying%20Kernels/box_blur.png">|<img width="240" height="300" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Applying%20Kernels/weighted_average_blur.png">|<img width="240" height="300" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Applying%20Kernels/gaussian_blur.png">    


 ### Sharpening Image
 Sharpening the image with 5x5 kernel without using inbuilt functions.
 Sharpening is opposite to the blurring. In blurring, we reduce the edge content and in Sharpening, we increase the edge content.     
 Original Image                     |  Sharpened Image
:-------------------------:|:-------------------------:
<img width="640" height="450" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Applying%20Kernels/sharpen_input.png">|<img width="640" height="450" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Applying%20Kernels/sharpen_output.png">


## Task 3
### Edge Detection
Edge detection is an image processing technique for finding the boundaries of objects within images. It works by detecting discontinuities in brightness.    
The explaination and kernel for Sobel Edge Detection can be found [here](https://www.cs.auckland.ac.nz/compsci373s1c/PatricesLectures/Edge%20detection-Sobel_2up.pdf).   
The explaination, code and steps for Canny Edge Detection can be found [here](https://towardsdatascience.com/canny-edge-detection-step-by-step-in-python-computer-vision-b49c3a2d8123
).     
 Original Image  | Vertical Edge Detection  | Horizontal Edge Detection
:-----:|:-----:|:-----:
<img width="340" height="340" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Edge%20Detection/edge-detection2.jpg">|<img width="340" height="340" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Edge%20Detection/v-edge2.png">|<img width="340" height="340" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Edge%20Detection/h-edge2.png">
  **Sobel Edge Detection**  | **Canny Edge Detection**
<img width="340" height="340" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Edge%20Detection/sobel2.png">|<img width="340" height="340" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Edge%20Detection/canny2.png">

## Task 4
### Morphology
Morphological transformations are some simple operations based on the image shape. It is normally performed on binary images. It needs two inputs, one is our original image, second one is called structuring element or kernel which decides the nature of operation. Two basic morphological operators are Erosion and Dilation.    
The complete explaination of erosion and dilation can be found [here](https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_imgproc/py_morphological_ops/py_morphological_ops.html
).      
Also, more information about use of padding the image can be found [here](https://medium.com/@ayeshmanthaperera/what-is-padding-in-cnns-71b21fb0dd7
).      
 Original Image  | Erosion  | Dilation  | Dilated Edge Detection
 :-----:|:-----:|:-----:|:-----:
 <img width="240" height="300" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Erosion%20%26%20Dilation/morphological.png">|<img width="240" height="300" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Erosion%20%26%20Dilation/Erosion.png">|<img width="240" height="300" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Erosion%20%26%20Dilation/Dilation.png">|<img width="240" height="300" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Erosion%20%26%20Dilation/Edge-Detection.png">
 
 
## Task 5
### Masking  
The complete information about masking of image for Colour Detection can be found [here](https://www.pyimagesearch.com/2014/08/04/opencv-python-color-detection/).   
Input Image                     |  Blue Ball Detection
:-------------------------:|:-------------------------:
<img width="640" height="450" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Masking/mask.jpg">|<img width="640" height="450" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/Masking/Blue%20Ball%20Detected.png">

## Task 6
### ROI extraction
We can extract the required part of image and using masking and bitwise operations, it can be added to the image in desired position.
The article for the same can be found [here](https://docs.opencv.org/3.4/d0/d86/tutorial_py_image_arithmetics.html).     
Input Image                     |  Output Image
:-------------------------:|:-------------------------:
<img width="640" height="450" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/ROI/roi.jpg">|<img width="640" height="450" src="https://github.com/Bhumika-Kothwal/Image-Processing/blob/master/ROI/ROI-output.png">

