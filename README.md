# FastAPI OCR

This project demonstrates an Optical Character Recognition (OCR) API using FastAPI and Tesseract-OCR. It provides a simple endpoint where users can upload an image, and the server will return the extracted text.

## Features

- **FastAPI** for creating a RESTful API.
- **Tesseract-OCR** for performing OCR on images to extract text.
- Upload images and receive extracted text as a response.

## Installation

Before you can run this project, you'll need to have Python installed on your system. This project was built using Python 3.8 or newer. You'll also need to install Tesseract-OCR and ensure it's available in your system's PATH.

### Step 1: Install Tesseract-OCR

Follow the installation instructions for Tesseract-OCR available at the [Tesseract GitHub repository](https://github.com/tesseract-ocr/tesseract). Ensure that the Tesseract executable is in your system's PATH so that it can be accessed by pytesseract.

### Step 2: Set up the Python environment

Clone this repository and navigate into the project directory. Create a virtual environment and activate it:

```bash
python -m venv env
env\Scripts\activate  # On Windows
source env/bin/activate  # On Unix or MacOS
```


### Step 3: Install required Python packages
Install the required packages using pip:

`pip install -r requirements.txt
`

### Running the Application
With all dependencies installed, you can run the server using:
`uvicorn main:app --reload
`
The FastAPI server will start, and you can view the API documentation by navigating to `http://127.0.0.1:8000/docs` in your web browser.


### Using the API
To use the OCR functionality:

1. Go to` http://127.0.0.1:8000/docs`.
2. Use the `/` endpoint to upload an image.
3. The API will return the extracted text as a response

