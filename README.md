# Face Recognition Code
This code provides an implementation of face recognition using the DeepFace library and OpenCV. It allows you to perform face recognition on both static images and real-time video from a webcam.

# Prerequisites
Before running the code, make sure you have the following dependencies installed:

- Python 3
- deepface library
- OpenCV
- matplotlib
- numpy

You can install the required dependencies by using the following command:

```
pip install deepface opencv-python matplotlib numpy
```

# Usage
The code consists of two main functions:

## 1. Face Recognition on a Static Image
The face_recognition function performs face recognition on a single static image. To use this function, follow these steps:

1. Set the path of the image you want to perform face recognition on by modifying the img variable. For example, img = "Data/elcan.jpg".
2. Specify the desired model and distance metric for face recognition by modifying the model_name and distance_metric arguments in the DeepFace.find method. The available options for models are defined in the models list, and the distance metrics are defined in the metrics list.
3. Call the face_recognition function. It will find the faces in the image, identify the people using the chosen model and distance metric, and display the original image with bounding boxes around the recognized faces. The identities of the recognized people will be printed.

## 2. Real-time Face Recognition
The realtime_face_recognition function performs real-time face recognition using the webcam. To use this function, follow these steps:

1. Call the realtime_face_recognition function.
2. A video capture window will open, showing the live video feed from your webcam. The code will continuously process each frame for face recognition.
3. Specify the desired model and distance metric for face recognition by modifying the model_name and distance_metric arguments in the DeepFace.find method. The available options for models are defined in the models list, and the distance metrics are defined in the metrics list.
4. Detected faces will be displayed with bounding boxes around them and the names of the recognized people overlaid on the video feed. The names are retrieved from the recognized identities.
5. Press the 'q' key to quit the program and close the video capture window.

# Configuration Options
The code provides several configuration options:

- backends: A list of available backends for face recognition. You can modify this list if you want to use a different backend.
- models: A list of available models for face recognition. Modify this list to choose a different model for recognition.

- metrics: A list of available distance metrics for face recognition. Modify this list to use a different distance metric.

Feel free to experiment with different models, backends, and distance metrics to achieve the desired face recognition results.

# Examples
Here are a few examples of how to use the code:

1. Perform face recognition on a static image:
```
img = "image.jpg"
face_recognition(img)
```
2. Perform real-time face recognition using the webcam:
```
realtime_face_recognition()
````
Remember to adjust the configuration options according to your needs.

# License
This code is provided under the MIT License. Feel free to use and modify it as per your requirements.

# Acknowledgments
The code utilizes the [DeepFace](https://github.com/serengil/deepface) library for face recognition, which is developed by serengil on GitHub. Please refer to their repository for more information about the DeepFace library.
