# Face detection model
 
The purpose of this project is to create a system for identifying faces in images. The project called for a model that could work
with reduced computational capabilities, so I opted for an SVC with a linear kernel. I then used Image Pyramid and Sliding Window to scroll through the image
on different scales so as to detect faces at different distances from the target. Finally, I provided a scikit-learn pipeline that takes an input image and returns a list with the coordinates of bounding boxes where faces are present; if there are no faces in the image, the list will be empty.