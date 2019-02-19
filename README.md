# Semi-Auto-Segmentation-Labelling-System
Author: Xu Liu
Date: 02/18/2019
This is a semi-auto labelling software for those who work on image labelling.   


Input: Click the "Open" button, open the "image" directory and select the first image to start. After this step, the left canvas will display the original image with 50% transparence colored label on it. And the right canvas will display the labelled image with totally black ground and colorful foreground (one color, one instance).  All the images in the "image" directory are the outputs(aka. prediction) of the segmentation deep neural network and are located at the "masks" directory. Most parts of the right image are labelled correctly by the neural network, what we need to do is just to revise it slightly.   


Instructions:  
1. Click your right mouse button on the right image to pick a color (the color is corresponding to the pixel where your cursor locates) that you wish to revise on the left image. If there are instances that have not been labelled, you can click your right mouse button on the circular color palatte to pick a different color.  

2. Move your cursor to right image, click at the place where you wish to revise the label, keep press the left mouse button and move it can draw curve lines, which can revise a large part.  

3. The silder on the top of the two images can control the pen (or brush) size, when you need to paint (revise) a large part, you can move the slider a bit right to get a larger pen size. On the other hand, just move it left can be helpful for revising small part.  

4. Click "Save" button on the right can save the revised image (the right one) as a 3 channels, 8 unsigned bits  PNG format file at the "output" directory, which is in the same directory as the "images" directory.   

5. Click "Next" button then the two canvas can refresh and load the next pair: image and label. Then just repeat the above operations.
