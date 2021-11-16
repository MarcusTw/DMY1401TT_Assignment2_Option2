# DMY1401TT_Assignment2_Option2

My classifier Web app hosted at [link](https://flaskapp-m4jbzqtwiq-uc.a.run.app/)
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


## Steps to Run Locally
1. Clone this repository
    ```sh
    git clone https://github.com/MarcusTw/DMY1401TT_Assignment2_Option2.git
    ```
2. (Optional) If you don't have Python, you can follow the guide to install Python 3.9.8 [here](https://www.python.org/downloads/release/python-398/). Do not use the latest Python 3.10 version as Tensorflow is not supported.

3. Install the required dependencies
    ```sh
    pip install -r requirements.txt
    ```
    or
    ```sh
    pip3 install -r requirements.txt
    ```
    
4. Lastly, you can run the application using Flask
    ```sh
    export FLASK_APP=app
    export FLASK_ENV=development
    flask run
    ```

5. (Optional) If you want to expose host and trust users on your network, you can make the server publicly available by adding --host=0.0.0.0 to the Flask run command.
    ```sh
    flask run --host=0.0.0.0
    ```
    Then you will be able to access the local server at [http://localhost:5000](http://localhost:5000).

6. Go to the hosted local server [http://127.0.0.1:5000](http://127.0.0.1:5000).
