# Chat with Images (OCR)

This application allows users to upload an image file and ask questions about its content. It uses Optical Character Recognition (OCR) to extract text from the image and then uses natural language processing to understand and respond to user queries based on the extracted text.

## Features

- Image file upload
- OCR text extraction from images
- Question answering based on extracted text
- Option to use either Google Palm (online) or Ollama (offline) for processing

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/chat-with-images.git
   cd chat-with-images
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

3. Install Tesseract OCR:
   - On Ubuntu: `sudo apt-get install tesseract-ocr`
   - On macOS: `brew install tesseract`
   - On Windows: Download and install from [GitHub](https://github.com/UB-Mannheim/tesseract/wiki)

4. Set up your Google API key in Streamlit secrets or as an environment variable.

5. If using Ollama, make sure it's installed and the "llama2" model is available.

## Usage

Run the Streamlit app:

```
streamlit run main.py
```

Then, open your web browser and go to the URL shown in the terminal (usually http://localhost:8501).

1. Use the sidebar checkbox to choose between Google Palm (online) and Ollama (offline).
2. Upload an image file using the file uploader.
3. Once uploaded, you can start asking questions about the image content in the text input box.

## Note

This application requires an active internet connection when using Google Palm. For offline usage, select the Ollama option.
