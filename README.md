# Prescription Scanning App

This is a simple Android application that allows users to capture an image using their device's camera, extract text from the captured image, and display the extracted text. The primary purpose of this app is to assist in scanning prescriptions or any other text documents.

## Features

- Capture image using the device's camera.
- Extract text from the captured image.
- Display the extracted text to the user.
- Permission handling for accessing the camera.

## Requirements

- Android device running Android OS version XX or above.
- Camera permissions granted for the application.

## Getting Started

To use this application, follow these steps:

1. Clone this repository to your local machine.
2. Open the project in Android Studio.
3. Build and run the application on an Android device or emulator.
4. Grant necessary permissions when prompted.
5. Tap on the "Capture Image" button to capture an image using the device's camera.
6. If prompted, allow the application to access the camera.
7. Once the image is captured, the application will extract text from the image and display it to the user.

## How It Works

- The main activity of the application (`MainActivity.kt`) initializes the camera capture functionality and sets up the UI for displaying the captured image and extracted text.
- The `extractTextFromImage()` function is responsible for extracting text from the captured image. It utilizes the Google Mobile Vision API for text recognition.
- The `createImageFile()` function creates a temporary image file to store the captured image.
- Permissions for accessing the camera are handled using the `ActivityResultContracts.RequestPermission()` launcher.
- The UI is built using Jetpack Compose, providing a modern and declarative way to build user interfaces.

## Dependencies

- Google Mobile Vision API for text recognition.
- Coil library for image loading and displaying.

## Limitations

- The accuracy of text extraction depends on the quality of the captured image and the clarity of the text.
- Currently, the application supports only the extraction of text from images captured in real-time. It does not support image selection from the device's gallery.



