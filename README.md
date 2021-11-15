# DMY1401TT_Assignment2_Option2

## Task Description
The task for this option is to deploy an object detection tool or service using existing pre-trained models.

The pretrained Object Detector and detection function can be found in the following [colab notebook](https://colab.research.google.com/github/tensorflow/hub/blob/master/examples/colab/object_detection.ipynb). Alternatively, you can use your own object detection model or code.

## Application
In this task, I have created a Web Service using Flask that allows user to input an image and be shown the image with boxes drawn to classify the objects.

### Server
1. Takes as input an image and displays or returns an image with bounding boxes drawn.
2. Communication between client and server (Rest API) must be in JSON format.

### Client
1. Web client that takes as input an image path and uploads/sends that image to the server.
2. Receives JSON response from server with the image with the plots itself.