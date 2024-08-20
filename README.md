# Image Classification App

This is a simple web application for image classification using a pre-trained MobileNetV2 model. The application allows users to upload an image and get predictions on the top-3 possible classes for the image. The app is built using Streamlit.

## Demo

You can try the app live [here](https://imageclassificationwebapp-h3qz2cmjyr6aurtjpwep7g.streamlit.app/).

## Features

- Upload images in `.jpg`, `.jpeg`, or `.png` format.
- Classify the image using the MobileNetV2 model.
- Display top-3 predicted classes with their respective probabilities.
- Show a horizontal bar graph of the prediction probabilities.

## How It Works

1. **Image Upload**: Upload an image through the sidebar.
2. **Image Preprocessing**: The uploaded image is resized to 224x224 pixels and preprocessed to match the input requirements of the MobileNetV2 model.
3. **Image Classification**: The preprocessed image is fed into the MobileNetV2 model, which predicts the top-3 possible classes.
4. **Results**: The predicted classes and their probabilities are displayed, along with a bar graph visualizing the probabilities.

## Installation

To run this app locally, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone <your-repo-url>
    cd <your-repo-directory>
    ```

2. **Install the required libraries**:
    ```bash
    pip install streamlit tensorflow pillow numpy matplotlib
    ```

3. **Run the application**:
    ```bash
    streamlit run app.py
    ```

## Code Overview

- **app.py**: The main script containing the Streamlit app code.
- **preprocess_image**: A function to resize and preprocess the image for the MobileNetV2 model.
- **classify_image**: A function to classify the preprocessed image and return the top-3 predictions.
