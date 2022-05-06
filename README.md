# devise_gesture_detection
This is a tinyML project that uses the built-in Accelerometer of a smartphone to classify gestures created by moving the phone via an NN model. For now, there are four types of gestures supported that are- Left-Right, Up-Down, Circle, and Idle

Edge Impulse Project URL: https://studio.edgeimpulse.com/public/103119/latest

## 1.Prerequisite
* A smartphone with built-in accelerometer and active internet connection.

## 2. Using the Classifier on Your Smartphone

There are two (2) steps to use this NN model on your smartphone
1. Connecting your smartphone to the project
2. Classification of device gestures using the model

### 2.1 Connecting your smartphone to the project
* To connect your smartphone simply scan the QR code below and open up the link in your preferred browser-

![unknown](https://user-images.githubusercontent.com/81281780/167143428-8d6b93ab-1998-437b-ba3e-59c2af7b4de3.png)

* Wait untill the model is completly downloaded once into your browser and make sure you have active internet connection

### 2.2 Classification of device gestures using the model

* Once the model is properly downloaded, it should notify you that your phone is connected with various options.
* Click on "Switch to classification mode". Then the device should start sampling.
* While sampling move your device in the following patterns. Make sure the bottom edge of your phone is facing towards you.

![Presentation1](https://user-images.githubusercontent.com/81281780/167147610-07df5f76-6a50-4ebc-a332-5fa475409012.png)

* During sampling periods, you can find your gestures calssified into one of the four aforementioned classes. The one with the highest probability (max 1), will imply the geasture. There is also a score designated for anomalies.

![IMG_20220506_200557](https://user-images.githubusercontent.com/81281780/167149305-50199a93-8401-445f-8932-f957e20c987c.jpg)

## 3. Deploying the Project on Arduino
You can deploy this project on an arduino (Preferrably Arduino Nano 33 BLE Sense) using the library included in this repository. however, it is not recommended as the data were collected using a smartphone.

## 4. Using the Model on an Embedded System
This repository also includes the TensorFlow Lite version of the NN model used in this project


## 5.Possible Applications
* Gesture based application development
* Motion analysis
