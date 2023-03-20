# Brain-Tumor-Segmentation-using-Watershed
This project aims to segment brain tumor MRI images using the watershed method. 
Watershed segmentation has a way of working by assuming that the image is a topography that 
will be filled with water and there are boundaries that separate each valley. In segmentation, 
the way it works is to look for the watershed line, namely the line with the highest point of the 
image delineation to the x and y positions. The x and y positions are the ground plane and pixel 
color intensity. The watershed algorithm is identical to a basin or valley which contains water 
and is delimited for certain parts. This algorithm works by interpreting the pixel intensity of 
the image as high. The basin of the valley will be filled with water and the boundary that 
touches will be given a boundary (ridge lines) and in this case the ridge lines are defined as the 
edges of the object. Then from each valley separated by ridge lines will be a different label. 
The steps in this algorithm are: 
1) separate objects of interest, 
2) convert the mask into intensity 
profile using the distance transform, 
3) run watershed algorithm, and 
4) update the original mask.
