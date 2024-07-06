# Tomato Plant Leaf Disease Classification

Welcome to the **Tomato Plant Disease Classification** repository! , this project leverages cutting-edge computer vision and machine learning technologies to enhance Tomato Leaf Disease Classification.

## 📄 Introduction
This code sets up a FastAPI server that utilizes a pre-trained TensorFlow model to classify images uploaded via API into different classes of Tomato Leaf diseases.
The primary objectives is:
- Detect the Disease in Tomato Leaf.

The system integrates CNN Architecture to detect disease in leaf.

## 🗂 Table of Contents
- [Introduction](#-introduction)
- [Requirements](#-requirements)
- [Demo](#-demo-video)
- [Features](#-features)
- [API Integration](#-server-access-using-postman-software)
- [Conclusion](#-conclusion)
- [Get Started](#-get-started)

## 📦 Requirements
1. [Numpy](https://numpy.org/doc/)
2. [uvicorn](https://www.uvicorn.org/)
3. [PIL (Pillow)](https://pillow.readthedocs.io/en/stable/)
4. [Tensorflow](https://www.tensorflow.org/api_docs)
5. [FastAPI](https://fastapi.tiangolo.com/tutorial/)
6. [Postman Software](https://learning.postman.com/docs/introduction/overview/)

## 🎥 Demo Video
https://github.com/AmanStarLitePro/Tomato-Leaf-Classification/assets/143260479/18335342-4159-47cf-b644-4f5eca557eec

## 🎯 Features

**Ping Endpoint**
- Responds with "Server is Ready" to indicate the server status.

**Predict Endpoint**
- Accepts an image file via POST request, processes it using a pre-trained TensorFlow model (my_model.keras), and returns the predicted class and confidence score of the image.

**Output**
- The model outputs predicted class and confidence of prediction.

## Server Access Using Postman Software

- API accessible via the local host server at `http://localhost:8000`.

- Install Postman:

- If you haven't already, download and install Postman from [here](https://www.postman.com/downloads/).
- Create a New Request:

- Open Postman and click on New to create a new HTTP request.
- Set the Request Type and URL:

- Select POST as the request type.
- Enter the API endpoint URL: http://localhost:8000/predict.

- Set Headers:
- Add a new header with key 'Content-Type' and value 'multipart/form-data'. 

- Set the Body:
- Click on the Body tab and Select the "form-data" option.
- Add a new key-value pair where the key is file (must match the parameter name file in your FastAPI endpoint) and the value is the image file you want to classify. You can either drag 
  and drop the image file or select it using the file picker.

- Send the Request:
- Click on Send to submit your request to the API.

- You should receive a response with the predicted class and confidence of prediction.

For more details on using Postman, refer to the [Postman Documentation](https://learning.postman.com/docs/introduction/overview/).

## 🏁 Conclusion

In this project, the FastAPI-based server developed in Python leverages a TensorFlow model to predict classes for tomato plant diseases with 89% accuracy. The server handles image uploads, processes them using a pre-trained convolutional neural network, and returns the predicted disease class along with its confidence level. This implementation provides a robust framework for real-time disease detection in agricultural settings, showcasing the integration of deep learning models within web applications for practical use.

Future work will focus on improving the models’ accuracy, expanding the dataset, and exploring additional functionalities to enhance the system’s capabilities.

## 🚀 Get Started

**Install Dependencies and Run the API:**

```sh
pip install -r requirements.txt
python Api/main.py

## Access the API:
Open your browser and go to http://localhost:8000/ping.


Thank you for checking out our project! If you have any questions or feedback, feel free to reach out to us.

