# Android Image Upload to Firebase Storage

This repository contains a simple Android project that demonstrates how to upload an image from the device's gallery to Firebase Storage using Java.

## Overview

This Android project showcases the process of selecting an image from the device's gallery and uploading it to Firebase Storage. The app allows users to choose an image, which is then uploaded to a designated folder on Firebase Storage.

## Prerequisites

Before you begin, make sure you have the following:

- Android Studio installed on your machine
- A Firebase project set up with the necessary configuration files added to your Android project

## Getting Started

1. Clone this repository to your local machine using:

```shell
git clone https://github.com/Divyakumar21202/Uploading_Img_FB.git
```

2. Open the cloned project in Android Studio.

3. Make sure you have your Firebase configuration files (`google-services.json`) added to the `app` module.

4. Run the app on an emulator or a physical device.

## How It Works

1. The app's main functionality is implemented in the `MainActivity.java` file.

2. The `openGallery` method is triggered when the user clicks the "Select Image" button. This method opens the device's image gallery using an intent.

3. Upon selecting an image from the gallery, the `onActivityResult` method is called. Here, the chosen image's URI is obtained, and the selected image is displayed in the `ImageView`.

4. When the user clicks the "Upload Image" button, the `upload_btn` click listener initiates the image upload process.
5. The image's URI is used to create a reference in Firebase Storage, and the `putFile` method is used to upload the image.

6. The `uploadTask` monitors the upload process, displaying a success or failure message accordingly.

## Usage

1. Launch the app on your Android device or emulator.

2. Click the "Select Image" button to open the image gallery.

3. Choose an image from the gallery.

4. After selecting an image, click the "Upload Image" button to upload the image to Firebase Storage.

## Important Note

Make sure you have set up Firebase correctly and added the required configuration files to your project before running the app.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to explore, modify, and use this code as a starting point for your own Android projects involving image uploads to Firebase Storage. If you have any questions or suggestions, please feel free to contact the author.
