PDF-to-Audiobook Converter
A research-based Python tool that converts any PDF document into an MP3 audiobook. 
Unlike standard converters that fail on scanned documents, this project implements a Hybrid Logic:
1. It attempts fast standard extraction first.
2. If it detects "Noisy" or "Image-based" pages (low character count), it automatically switches to **AI Vision (OCR)**.

🚀 Key Features
Adaptive Switching: Automatically detects if a page is text or an image.
Hybrid Engine:Combines `PyPDF2` (Speed) + `Tesseract-OCR` (Accuracy).
Universal Support:Works on typed PDFs, scanned notes, and book photos.
Audio Output:Uses Google Text-to-Speech (gTTS) for clear narration.

Tech Stack
Language: Python 3.10
Core Logic: PyPDF2 (Text Parsing), Tesseract (OCR Vision).
Audio: gTTS (Google Text-to-Speech).
System: Google Colab Environment.

⚙️ How to Run
Open the .ipynb file in Google Colab.
Run the installation cell to set up the OCR environment.
Upload any PDF (even a scanned one).
The script will analyze the file type and generate the audio automatically.
