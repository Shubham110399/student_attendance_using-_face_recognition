Facial Recognition-Based Attendance System
Project Overview
This project is a full-stack web application designed to automate the attendance process using real-time facial recognition. By replacing manual registers with automated identification, the system significantly reduces administrative time and eliminates manual data entry errors.

Key Features

Real-time Detection: Captures and processes video frames instantly to identify registered individuals.


Secure Authentication: Integrated a Flask backend to handle secure user requests and system logic.


Persistent Storage: Utilizes a MySQL database to manage user profiles and maintain historical attendance logs.


User Dashboard: A responsive web interface built with HTML/CSS for easy user registration and attendance report viewing.

Technical Stack

Language: Python 


Libraries: OpenCV (Image processing), face_recognition (Deep Learning-based embeddings) 


Frameworks: Flask (Backend), Bootstrap (Frontend) 



Database: MySQL 

How It Works (Technical Logic)

Image Processing: The system uses OpenCV to access the camera feed and detect facial bounding boxes.


Feature Extraction: It generates 128-d face embeddings using the face_recognition library to represent unique facial features as mathematical vectors.


Matching: The system calculates the Euclidean distance between the live face and the database of stored embeddings; a match is recorded if the distance is below a specific threshold.


Logging: Upon successful recognition, the system automatically updates the MySQL database with a timestamp and the user’s ID
