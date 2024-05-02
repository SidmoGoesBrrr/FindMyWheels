
# FindMyWheels Project Overview

## Introduction
**FindMyWheels** is an innovative parking management system designed to help users locate their vehicles quickly and efficiently in parking lots. The system utilizes a mini robotic car equipped with cameras and sensors to capture images and details of parked vehicles, which are then processed to allow easy vehicle location and parking analytics.

This repository serves as a non-technical hub providing an overview of the entire FindMyWheels system, linking to individual component repositories which contain the actual source code and technical details.

## Components
FindMyWheels consists of several interconnected components, each residing in its own repository:

### 1. [FindMyWheels-Android](https://github.com/SidmoGoesBrrr/FindMyWheels-Android)
The Android application acts as the interface for the camera on the robotic car. It captures images triggered by the Arduino device and communicates with the backend to fetch and display available parking data.

### 2. [FindMyWheels-Backend](https://github.com/SidmoGoesBrrr/FindMyWheels-Backend)
The backend, developed in Python using FastAPI, handles data processing, storage, and retrieval. It processes the images captured by the Android app to extract vehicle details and stores this information in Firebase Realtime Database.

### 3. [FindMyWheels-Frontend](https://github.com/SidmoGoesBrrr/FindMyWheels-Frontend)
The frontend is a React-JS based dashboard that displays the parking lot maps and available vehicle information to the users, allowing them to easily locate their vehicle.

### 4. [FindMyWheels-Arduino](https://github.com/SidmoGoesBrrr/FindMyWheels-Arduino)
This repository contains the code for the Arduino that controls the mini robotic car. It includes functionalities for automatic movement, sensor data processing, and Bluetooth communication to trigger the camera on the Android app.

## System Flow
- **Startup:** The robotic car starts and begins navigating the parking lot.
- **Detection:** When the car's IR sensors detect a predefined marker, it stops and signals the Android app to capture an image.
- **Image Processing:** The Android app sends the captured image to the backend, where vehicle details are extracted and stored.
- **Data Utilization:** The frontend dashboard utilizes this data to display vehicle locations and additional parking analytics to the users.

## Non-Technical Details
This project aims to simplify the parking experience using technology, making it easier to manage large parking lots and saving time for users. The integration of different technologies such as Arduino for robotics, Android for mobile development, and Python for backend processing showcases a multidisciplinary approach to solving real-world problems.
