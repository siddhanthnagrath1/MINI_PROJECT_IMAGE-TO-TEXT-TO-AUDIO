
# Image to Text to Audio Converter

### Project Type: University Homework Assignment  
### Format: Jupyter Notebook (`.ipynb`)  
### File: `Image_to_text_to_audio.ipynb`

---

## Overview

This project demonstrates a basic pipeline to convert an image with text into an audible speech format. The pipeline performs three main operations:

1. **Image-to-Text**: Extracts text from an input image using Optical Character Recognition (OCR).
2. **Text Processing**: Cleans and optionally processes the extracted text.
3. **Text-to-Speech**: Converts the text into speech using a TTS (Text-to-Speech) engine and plays or saves the audio.

---

## Technologies Used

- **Python**
- **Tesseract OCR** (`pytesseract`)
- **Text-to-Speech** (`gTTS` or `pyttsx3`)
- **Jupyter Notebook**

---

## Setup Instructions

### 1. Clone or download the notebook
```bash
git clone https://github.com/siddhanthnagrath1/MINI_PROJECT_IMAGE-TO-TEXT-TO-AUDIO
```

### 2. Install Required Libraries
Use pip to install dependencies:
```bash
pip install pytesseract pillow gTTS pyttsx3
```

### 3. Install Tesseract OCR engine
- For Windows: [Download from GitHub](https://github.com/tesseract-ocr/tesseract)
- For Linux:
```bash
sudo apt-get install tesseract-ocr
```

---

## How to Run

1. Open the Jupyter Notebook:
```bash
jupyter notebook Image_to_text_to_audio.ipynb
```

2. Upload an image containing text.

3. Run all cells:
   - The text will be extracted from the image.
   - The extracted text will be converted into audio and either saved or played.

---

## Example Workflow

```python
# Load image and extract text
image = Image.open('example_image.jpg')
text = pytesseract.image_to_string(image)

# Convert to audio
tts = gTTS(text)
tts.save("output.mp3")
```

---

## Project Files

- `Image_to_text_to_audio.ipynb` – Main notebook containing code and explanations.
  

---

## Author

This project was developed as part of a university homework assignment to demonstrate OCR and speech synthesis capabilities using Python.
