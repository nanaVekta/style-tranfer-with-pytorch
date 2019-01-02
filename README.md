# style-tranfer-with-pytorch
The main goal of project is to combine two images and produce new image. The combination works in slightly different way i.e., we combine the style of one image with the content of other image. First we take the image from which we want to extract content usually called **content image** and take another image from which the style is to be extracted usually called **style image**.

Convolutional Neural Networks are a type of neural networks which are used widely in Image classification and recongnition. A CNN architecture called **VGG19** has been used in this project. The starting layers in this architecture extract the basic features and shapes and later layers will extract more complex image patterns. So for the output image we will take the content from later layers of CNN. For extracting the style of image, we take the correlations between different layers using Gram Matrix

Initially, we take any random image as target(or taking the content image would be useful) and compute the Content loss and Style loss and decreasing these losses we would reach the perfect target image that has the style of one image and content of other image. For more learning checkout the links below.

**Note: The notebook has been ran on Google Colab, If you are working on local machine, the starting four cells can be ignored. To use this and produce new styled images, just change the links to the style and content variables, change the path in the last cell, and include the path where you want to save the styled image and run the entire notebook.**

In this project I used:
1. Python: language
2. NumPy: library for numerical calculations
3. Matplotlib: library for data visualisation
4. PIL: Python Image Library for opening and manage different image formats
5. torch: a deep learning framework by Facebook AI Research Team
6. torchvision: package consists of popular datasets, model architectures, and common image transformations for computer vision
