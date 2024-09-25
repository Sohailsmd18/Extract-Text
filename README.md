This project demonstrates a web application that allows users to upload an image containing both Hindi and English text. The application performs Optical Character Recognition (OCR) on the image to extract the text and includes a keyword search functionality within the extracted text.

Features
Image Upload: Users can upload an image in common formats (JPEG, PNG, etc.).
Text Extraction: The app uses OCR to extract text from images containing Hindi and English text.
Keyword Search: Users can search for specific keywords in the extracted text and see results with highlighted keywords.

Technology Stack
Backend OCR:
Pytesseract (or Huggingface Transformers if required)
Tesseract OCR for text extraction.

Frontend:
Streamlit or Gradio for the web interface.
Installation and Setup

Prerequisites:
Python 3.10+
Tesseract OCR installed on your system.
Install the required Python libraries.


Instructions:

Clone the repository:
git clone <repository-url>
cd ocr_web_app


Install required dependencies:
pip install -r requirements.txt


Set Tesseract Path (Windows only): Add the following in ocr.py (already included):
pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'


Run the Application:
For Streamlit:
streamlit run app.py

For Gradio:
python app.py

Deployment
You can deploy the app to:
Streamlit Cloud for Streamlit-based applications.
Huggingface Spaces for Gradio-based applications.


Example Use Case
Upload an image: Upload an image containing Hindi and English text.
Text Extraction: The OCR processes the image and displays the extracted text.
Search Functionality: Enter a keyword to search within the extracted text.