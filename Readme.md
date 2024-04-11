# ATS Resume Scanner

## Overview

The ATS Resume Scanner is a Streamlit application designed to assist in the evaluation of resumes against job descriptions. It utilizes a generative AI model from Google to analyze the content of a resume and provide feedback or a percentage match with the job description.

## Installation

Before running the application, ensure you have the following all libraries installed given in requirements.txt

You can install these libraries using pip:

```bash
pip install requirements.txt
```

## Configuration

Set up your environment variables by creating a .env file in the root directory and adding your API key:

```bash
your_api_key='YOUR_API_KEY_HERE'
```

## Usage

To start the application, run the following command:

```bash
streamlit run app.py
```

## Functions

get_gemini_response(input, pdf_content, prompt): This function sends the input, the first page of the PDF content, and the prompt to the generative AI model and returns the generated text response.
input_pdf_setup(uploaded_file): This function converts the uploaded PDF file into an image of the first page, encodes it to base64, and prepares it for the AI model.
Streamlit App
The Streamlit app (app.py) provides a user interface for uploading resumes (PDF format) and entering job descriptions. It offers two functionalities:

Tell Me About the Resume: Evaluates the resume and provides a professional evaluation against the job description.
Percentage Match: Calculates the percentage match of the resume with the job description and lists missing keywords and final thoughts.
