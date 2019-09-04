# Digital-image-analysis

This python script contains functions for image analysis and transformation. The script uses openCV, matplotlib and numpy. OpenaCV is used for reading and writing images.

ImportPic function is helper function that accepts two arguments, image path and mode. Argument mode is int variable that determines wether the image is diretly read as gray scale image. Image will be read as gray scale image when mode = 0. If we want to read image in color the mode needs to be 1 (default value). When an image is read with mode 0 it is convertet into numpy 2D array where the color is expresed as a singel value, but when the image is read with mode 1 then the color represented as RGB value in form of array with length of 3.

Functions

1) connvertToGrayScale accepts two arguments, image path and boolean value. If the boolean values is true then the image is shown and returned otherwise it's not shown.

2) createHistogram creates histogram that show the number of pixcels of certain value. This function accepts five arguments, image path, pic, cumulative, show_pic and show_hist. This function can accept path to an image or image that has previously imported, for this purpose arguments image path and pic are used. Argument cumulative is boolean values that determines will the histogram be cumulative or not. Boolean argument show_pic and show_hist determine wether to show image and histogram or not.

3) normalizeHistogram spreads image histogram over the whole range of values (0-255) which has the effect of adding contrast to the image. This function has two arguments, image path and show_pic. Argument show_pic accepts the boolean value and determines wether or not the path image will be shown. Normalized histogram is always show.
