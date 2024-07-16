# Image-Annotation-without-using-Object-Detection-Model
Developed a Python algorithm using image processing techniques to partially de-annotate images by removing specific annotations without re-annotating the original image. Employed OpenCV and dynamic bounding box expansion to achieve efficient and scalable results, ensuring preservation of the original image's integrity.
Data
● original_image: Original Base Image without annotation 
● fully_annotated: Fully annotated Image
● partially_annotated: Partially annotated Image
Techniques Used
Image Resizing: The original image is 978×978 pixels and The fully annotated image is 938×939 pixels.
Open CV: Haar Cascade Classifier is used for detecting cat faces in the grayscale image.
The detection parameters are tuned to ensure only one cat face is detected, which helps avoid false positives.
https://pyimagesearch.com/2016/06/20/detecting-cats-in-images-with-opencv/
Dynamic Bounding Box Expansion: Bounding box around cat face is dynamically expanded, and checks for similar pixels to mark the area of interest.
Mask Creaton: mask the area of interest on fully annotated image.
Result: The difference between Original and Fully annotated image is taken to create the Partially annotated image.
Documentation:
Open CV: haarcascade_frontalcatface_extended.xml 
Numpy
Matplotlib
