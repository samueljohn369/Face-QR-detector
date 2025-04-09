# Face-QR-detector
An Android app that combines real-time face detection and QR code scanning using ML Kit and cameraX.

This is an Android application developed using Android Studio that combines real-time face detection and QR code scanning in a single app. It leverages Google's ML Kit for face detection and either ZXing or ML Kit Barcode API for QR scanning, providing smooth and fast camera-based features.

The app has a clean UI with two main options:

1.Open QR Scanner – Launches a camera view to scan QR codes and retrieve data instantly.

2.Open Face Detection – Opens a camera view that detects human faces in real time and draws bounding boxes.

The project is structured in a modular way with separate packages for face detection and QR scanning. It uses CameraX to handle camera operations efficiently.

This app is ideal for beginners and intermediate Android developers looking to explore computer vision features like face tracking and QR decoding in a real-world Android project.



PROJECT STRUCTURE 

![Screenshot 2025-04-09 122853](https://github.com/user-attachments/assets/cbf102a1-61bc-45bf-a28d-cb13ba72e8c7)




1. facedetector/
   
     Purpose: Implements real-time face detection using Google's ML Kit.

     Key Files:

     FaceBoxOverlay.java: Draws bounding boxes around detected faces on the camera preview.

     FaceDetectionActivity.java: Manages camera input and face detection logic.

2. facemeshdetector/
   
     Purpose: (Optional) Adds support for face mesh detection, mapping facial features in more detail.

     Key File:

     FaceMeshDetectionActivity.java: Launches a face mesh detector using ML Kit’s face mesh API.

3. qrscanner/
   
     Purpose: Handles QR code scanning functionality using CameraX and ZXing/ML Kit.

     Key Files:

     ScannerActivity.java: Opens the camera view to scan QR codes.

     CameraXViewModel.java: Manages camera lifecycle and setup using ViewModel.

     Action.java: (Utility/helper class) Possibly defines QR code actions.

     Utils.kt: Helper functions for QR processing or display.

4. Root Files
   
     MainActivity.java: The main screen with buttons to launch either QR scanning or face detection.

     AndroidManifest.xml: Registers activities and defines app permissions (like camera access).

     build.gradle: Declares dependencies like CameraX and ML Kit.

5. res/layout/
   
     XML Layouts that define the UI for each screen:

     activity_main.xml: Main screen with buttons.

     activity_face_detection.xml: UI for face detection view.

     activity_face_mesh_detection.xml: UI for face mesh detection (if used).

     activity_scanner.xml: UI for QR code scanning.





   INTERFACE



   ![Screenshot 2025-04-09 123733](https://github.com/user-attachments/assets/825da8a4-0b64-4c31-8431-c48e9ec8d87a)





