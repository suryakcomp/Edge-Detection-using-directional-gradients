# Edge-Detection-using-directional-gradients
This is a MATLAB demo to elaborate the idea of boundary tracing objects in image using directional gradients

In any image the edges lie where the rate of change in the intensity value of the pixel is sudden & high. Building on this idea I have been trying to detect a nucleus and trace its boundary in a cell image automatically by just clicking on the nucleus. By the click, a point (pixel) is selected through which a family of lines is originated. In terms of pixels, start converting the pixels to white in radially outward direction from the selected point. Now for each direction we keep on recording the difference between the original pixel value and the white turned pixel value which can be defined as directional gradient at that pixel. When a sudden change in the value of directional gradient is recorded, based on a threshold value the line in that direction is terminated and hence the boundary/edge is detected. I have been working on this idea and developed some initial codes in matlab to give a proof of concept with limited results.  

createGrayImage.m         -> demo image for testing ;
generateDirections.m      -> demo to generate different directional vectors ;
directionalCrossSection.m -> final code
