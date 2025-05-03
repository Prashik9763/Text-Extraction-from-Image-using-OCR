# 📖 Text Extraction from Images using OCR

The **Text Extraction from Images using OCR** is a Python-based desktop application that lets users extract text from images using OCR, display the text, and fetch the meaning of individual words from an online dictionary API. The app also allows users to capture images using their camera, navigate through multiple imported images, and export the extracted text to Word and PDF formats.

## 🛠 Features

- 📸 **Image Import & Capture**: Import images or capture photos using a webcam.
- 🔤 **Text Extraction**: Extract text using Tesseract OCR.
- 🧠 **Word Meaning Fetcher**: Click on any word in the extracted text to get its meaning using the [Free Dictionary API](https://dictionaryapi.dev/).
- 🗃️ **Save Text**: Export the extracted content to `.docx` (Word) or `.pdf` format.
- 🔁 **Image Navigation**: Navigate between imported or captured images.
- 🖼️ **Image Display**: Preview currently selected/captured image in the GUI.

## 📦 Requirements

- Python 3.x
- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) (must be installed and its path configured)
- Required Python libraries:

```bash
pip install pytesseract pillow nltk opencv-python python-docx reportlab requests

⚙️ Setup
Install Tesseract OCR and update this path in main.py:

python
Copy
Edit
pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'
os.environ['TESSDATA_PREFIX'] = r'C:\Program Files\Tesseract-OCR\tessdata'
Download NLTK tokenizer (once):

python
Copy
Edit
import nltk
nltk.download('punkt')
