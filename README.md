# Image Upscaling Web App

This code repository contains a simple web page application that allows users to upscale an image and download the upscaled version. The application utilizes HTML, CSS, and JavaScript to achieve this functionality.

## Functionality

The web page provides the following features:

- **Image Selection:** Users can select an image file through a form input.
- **Preview Display:** A preview div displays the selected image.
- **Upscale Image:** Clicking the "Upscale Image" button enlarges the image.
- **Download Upscaled Image:** Users can download the enlarged image.

## Implementation Details

- **FileReader API:** Used to read the selected image file as a data URL.
- **Image Preview:** The FileReader sets the src attribute of a new img element, which is then appended to the preview div.
- **Upscaling Process:** When the "Upscale Image" button is clicked:
    - A new canvas element is created with dimensions eight times the original image's width and height.
    - The original image is drawn onto this canvas at a scale of 8 using the drawImage() method.
    - The original image is replaced with the upscaled version.
- **Download Functionality:** Clicking the "Download Upscaled Image" button:
    - Converts the canvas element to a data URL using toDataURL().
    - Creates a new anchor element with the download attribute set to the filename and href attribute set to the data URL.
    - Appends the anchor to the body and simulates a click, initiating the download.
    - Removes the anchor from the body after the download.

## How to Use

1. Clone the repository to your local machine.
2. Open the `index.html` file in a web browser.
3. Select an image file using the provided form.
4. Click the "Upscale Image" button to enlarge the image.
5. Use the "Download Upscaled Image" button to save the enlarged image to your device.

## Contributors

- isaiah wanyama

