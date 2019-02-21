# GraphicsPhotoshop
Miniature Photoshop which practices multiple fundamental image processing techniques. </br>
Options include: </br>
1. Color to Grayscale </br>
2. 24 to 8 bit Color </br>
3. Uniform Quantization (4 shades of blue, 8 shades of red, and 8 shades of green)</br>
4. Populosity: find the 256 most popular colors, then map the original colors onto their closest chosen color</br>
5. Dithering options: </br>
  (1) Dithering </br>
  (2) Naive Threshold Dithering: Dithering with a threshold of 0.5 </br>
  (3) Brightness Preserving Threshold Dithering: Using threshold dithering with a threshold chosen to keep the average brightness constant.</br>
  (4) Random Dithering: Adding random values chosen uniformly from the range [-0.2,0.2], assuming that the input image intensity runs from 0 to 1 (scale appropriately)</br>
  (5) Clustered Dithering: cluster dithering with the matrix shown below. The image pixels is compared to a threshold that depends on the dither matrix below. The pixel is drawn white if: I[x][y] >= mask[x%4][y%4]. The matrix is: [0.7059 0.3529 0.5882 0.2353 0.0588 0.9412 0.8235 0.4118     0.4706 0.7647 0.8824 0.1176     0.1765 0.5294 0.2941 0.6471]</br>
  (6) Floyd-Steinberg Dithering: Dither using Floyd-Steinberg dithering (Distribution of error to four neighbors and zig-zag ordering).</br> 
  (7) Color Floyd-Steinberg Dithering: Quantize the original image(with color) and use Floyd-Steinberg dithering </br>
6. Filtering options:</br>
  (1) Box Filter (5x5)</br>
  (2) Bartlett Filter (5x5)</br>
  (3) Gaussian Filter (5x5)</br>
  (4) Arbitrary-Size Gaussian Filter (nxn)</br>
7. Image Resizing options: </br>
  (1) Half size</br>
  (2) Double size </br>
  (3) Arbitrary Uniform Scale scale</br>
  (4) Arbitrary Rotation </br>
8. NPR Paint Method: Simplified version of 1998 SIGGRAPH Paper "Painterly Rendering with Curved Brush Strokes of Multiple Sizes"(https://mrl.nyu.edu/publications/painterly98/hertzmann-siggraph98.pdf) Gives image an oil painting like effect.</br>



 
