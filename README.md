Image compression using K-Means clustering is a technique that reduces the number of distinct colors in an image while preserving its visual quality. 
Instead of storing millions of colors, the image is compressed by clustering similar colors into a fixed number of representative colors (called centroids).
The process involves:

Reshaping the Image: The image is converted from a 3D array (height × width × RGB) into a 2D array where each row represents a pixel's RGB value.
Clustering Colors: K-Means clustering groups the pixels into K clusters based on color similarity in RGB space.
Replacing Colors: Each pixel’s color is replaced with the centroid color of its cluster, effectively reducing the number of unique colors in the image to K.
Reconstructing the Image: The modified pixel values are reshaped back to the original image dimensions.
This approach significantly reduces the amount of data needed to store the image, making it ideal for lossy compression in applications like web graphics and thumbnails.
