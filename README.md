# CK12 Solver

This project utilizes Python and various libraries to interact with the Snipping Tool, capture an image, use Optical Character Recognition (OCR) to extract text from the image, and then obtain a response to the question from the OpenAI GPT-3 API.

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/snoopypoopsy/CK12-solver.git

2. **Install Dependencies**
   
   Ensure you have Python installed. This project was developed using Python 3.x.
   Install required Python packages using pip:
   ```bash
   pip install pyautogui pytesseract opencv-python openai pillow pyperclip

  Install Tesseract OCR and ensure it's in your system PATH.
  For Windows: Download and install Tesseract OCR from this link: https://github.com/UB-Mannheim/tesseract/wiki.
  For macOS: Use Homebrew and install with brew install tesseract.
  For Linux: Use your package manager to install Tesseract OCR, e.g., sudo apt-get install tesseract-ocr.

3. **API KEY**
   
   Obtain an API key from OpenAI GPT-3 and replace the placeholder **'api_key'** in the code with your actual key.

## How to Use

1. **Run the Python script**
   
   Open a terminal or command prompt. Navigate to the project directory. Run the command: **python solver.py**.
2. **Trigger the snipping tool and capture the image**
   
   The script will simulate the Win + Shift + S key combination to trigger the Snipping Tool. 
   Manually select the area you want to capture using the Snipping Tool.

3. **Observe the Process**

    The script will attempt to extract text from the captured image using OCR.
    It will then send a question prompt to the GPT-3 model.
    The AI will respond with an answer based on the extracted question.

## Disclaimer
**Use at your own risk**: This project is provided as-is and may not work perfectly in all scenarios or on all systems.

**Open AI API usage**: Ensure compliance with OpenAI's use policies and terms of service when using their API.

**User Interaction**: The project requires manual interaction for snipping selection and might be affected by variations in Snipping Tool behavior or OCR accuracy.
