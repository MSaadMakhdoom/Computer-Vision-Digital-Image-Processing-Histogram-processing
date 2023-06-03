# Digital-Image-Processing-Histogram-matching


# Digital Image Processing
## Solution
##  Enhance the image with Laplacian filters if they can find the hidden objects and show the results. Explain their success or failure. - Laplacian filters are used to enhance edges and detect edges in an image.

- The Laplacian filter works by finding the second derivative of the image intensity function. 
- It enhances areas of the image where the intensity changes quickly, such as edges or boundaries  
- different objects in the image. Therefore, Laplacian filters can be effective at revealing hidden objects in an image.


## Use any other spatial filtering techniques that you think is suitable to find the hidden objects.
- Load the image
- Convert the image to grayscale
- Apply a Laplacian filter to detect edges
- Apply a Sobel filter to detect edges in both directions
- Apply a Gaussian filter to smooth the image
- Threshold the Laplacian and Sobel images to obtain binary images
# Result
![Output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/raw/main/output/Screenshot%202023-06-03%20at%204.02.15%20AM.png)

## code that implements Mathematical formula enhance the image:
- Compute global mean and standard deviation
- Compute local mean and standard deviation using a square neighborhood
- Compute enhanced image using the given formula
![Output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/output/Screenshot%202023-06-03%20at%204.02.32%20AM.png)
##
# Result
![Output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/output/Screenshot%202023-06-03%20at%204.02.41%20AM.png)
## Find only the blue board that has text and arrow signs. The rest of the pixels in the image should be black
# inputimage
![input](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/data/road.jpg)
- Read the image
- Calculate the histogram
- Draw the histogram
- Check if the image is too dark or too bright
- Apply histogram equalization
- Calculate the histogram of the equalized image
- Display the equalized image

- Load the image
- Convert the image to HSV color space
- Define the range of blue color in HSV
- Create a mask for the blue board
- Perform morphological operations to remove noise
- Find contours in the image
- Loop over the contours and find the blue board that has text and arrow signs
- Create a black image of the same size as the original image
- Draw the blue board on the black image
- Add the black image to the list
- Combine all the black images using bitwise OR operation
- Mask the original image with the black image to make the rest of the pixels␣
# preprocessing image
![output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/output/Screenshot%202023-06-03%20at%204.02.58%20AM.png)
# result
![output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/output/Screenshot%202023-06-03%20at%204.03.07%20AM.png)
#
## Write a program that should be able to find the background color of the sign board. It should be a generic function to identify three different primary colors: red, green or blue. It should display blue if the background color of the board is blue

- initializes a variable named "blue_count" to 0.
- It loops through each pixel in the image using two nested for loops.
- For each pixel, it unpacks the RGB values into three separate variables named "r", "g", and "b".
- It checks whether the blue value of the pixel (b) is greater than both the␣ red value (r) and the green value (g). If it is, it increments the␣ "blue_count" variable.
- After all the pixels have been processed, it calculates the percentage of blue pixels in the image by dividing the "blue_count" variable by the total number of pixels in the image (width times height).

- If the percentage of blue pixels is greater than 50%, the function returns␣the string "blue". Otherwise, it returns the string "not blue"


#### Apply thresholding to show text shown in the sign board along with arrow signs in black while the background of the sign board and rest of the image in white. You should find the threshold value automatically by calculating a histogram. The histogram ideally will have two peaks, select the value in between two peaks as the threshold value. If you use your manually entered threshold then NO MARKS will be assigned for this part

- Read in the image
- Calculate the histogram of the image
- Find the two peaks in the histogram
- Apply thresholding to the image
- Invert the thresholded image so that text and arrow signs are black
![output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/output/Screenshot%202023-06-03%20at%204.03.16%20AM.png)

## Problem 3
Write a function that takes two images as input and display “Similar” if two images are similar
otherwise display “Different”.
#
![output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/output/Screenshot%202023-06-03%20at%204.04.45%20AM.png)

## Problem 4
# part a. Apply a global threshold on the above images and see the output. Probably it will fail. Explain your reasons for failure of the global thresholding.


![output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/output/Screenshot%202023-06-03%20at%204.04.59%20AM.png)

## part b Local Thresholding: In local thresholding we will select a small window and then apply a thresholding with respect to that small window. You can try implement your own custom function for the following technique to see if local thresholding will work.
![output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/output/Screenshot%202023-06-03%20at%204.05.08%20AM.png)

## part c In OpenCV Adaptive Thresholding is provided. Undersand the working of Adaptive Thresholding. You can try adaptive thresholding and display your results. Compare and comment on the results obtained for your method, adaptive method and global thresholding method. Which seems more suitable for the above images.
![output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/output/Screenshot%202023-06-03%20at%204.05.47%20AM.png)

## problem 5
## input image
![output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/data/fundus.jpg)
A normal fundus image of human eye is shown in figure 5. Perform the following tasks:
# a. Separate the veins in the eye and display them (rest of the pixels in black veins in white)
# b. Find the diameter of the eye ball (shown with arrow) in terms of pixels and display it.

![output](https://github.com/MSaadMakhdoom/Digital-Image-Processing-Histogram-matching/blob/main/output/Screenshot%202023-06-03%20at%204.05.57%20AM.png)







