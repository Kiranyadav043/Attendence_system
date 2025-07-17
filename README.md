Smart Attendance System Using Facial Recognition
This project is a smart attendance tracking system that leverages facial recognition to automate the process of marking attendance. The system allows users to register their face, log in using face authentication, and automatically records login and logout times. It is built using computer vision, machine learning, and is designed with modular and scalable code practices following object-oriented programming principles.

Features
Face Registration
Captures 300 facial samples per user using MediaPipe FaceMesh (468 landmarks).

Stores landmark data and corresponding labels for training.

Automatically retrains the recognition model after each registration to include new users.

Real-Time Face Recognition
Uses a trained RandomForestClassifier to recognize users in real-time through webcam.

Facial features are preprocessed and normalized for accurate classification.

Employs LabelEncoder to manage user labels efficiently.

Automated Attendance Logging
Detects and logs:

Login Time

Logout Time

Total Working Hours

Login Status (e.g., On Time or Late based on configurable threshold)

Attendance is saved in a structured CSV format.

Reporting
Daily reports are automatically generated and saved in the attendance/ directory.

Reports include columns: Name, Login Time, Logout Time, Working Hours, and Login Status.

Menu-Driven Interface
A terminal-based menu allows users to:

Register new faces

Mark attendance

View attendance reports

Exit the program

Modular and Maintainable Codebase
Implements object-oriented programming for better structure and reusability.

Clean separation of responsibilities between registration, recognition, and reporting modules.

Technologies Used
Python

OpenCV

MediaPipe FaceMesh

scikit-learn (Random Forest Classifier)

pandas

