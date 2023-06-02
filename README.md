# Digital-Image-Processing-Histogram-matching


# Digital Image Processing
## Solution
##  Enhance the image with Laplacian filters if they can find the hidden objects and show the results. Explain their success or failure. - Laplacian filters are used to enhance edges and detect edges in an image.
# input image
![Squares Image](data/squares.tif)

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
! [Output](.\output\Screenshot%202023-06-03%20at%204.02.15%20AM.png)
## code that implements Mathematical formula enhance the image:
- Compute global mean and standard deviation
- Compute local mean and standard deviation using a square neighborhood
- Compute enhanced image using the given formula

## Find only the blue board that has text and arrow signs. The rest of the pixels in the image should be black

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

## Problem 3
- Convert image to grayscale if not already in grayscale
- Calculate gradient magnitude and direction
- Define threshold for angle
- Define kernels for different orientations
- Filter image with kernel and angle threshold
- Threshold the image to convert it to black and white

#### Find percentage of the area covered by the hexagon and display it.

- Create a histogram of the pixel intensities
- Plot the histogram as a bar graph
- Add labels to the plot










