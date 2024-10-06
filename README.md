# Financial Document Information Extraction

![Financial Document Information Extraction cover image](./Cover.png)

This project automates the extraction of key details from financial documents like invoices, receipts, and bills using Optical Character Recognition (OCR) and LayoutLM-based document classification.

## Features

- **Image Processing**: Handles multiple image formats (PNG, JPEG, TIFF, etc.) and converts them to grayscale.
- **Optical Character Recognition (OCR)**: Extracts text from images using Tesseract OCR.
- **Document Classification**: Classifies documents into predefined categories using LayoutLM, a state-of-the-art model for document understanding.
- **Information Extraction**: Extracts important financial details such as numeric values and dates.
- **CSV Storage**: Saves the extracted data, including document details, predicted labels, and accuracy, into a CSV file for easy review and analysis.

## How It Works

1. **Load Images**: The system reads images of financial documents from a specified directory.
2. **OCR Process**: The images are converted to text using OCR.
3. **Document Classification**: The extracted text is used to classify the document type.
4. **Information Extraction**: Key financial data, like amounts and dates, are extracted from the text.
5. **Store Data**: The extracted information is saved in a CSV file for further use.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/priyasingh26/Financial_Document-Data_Extraction.git
2. Install required Libraries:
   ```bash
   pip install -r requirements.txt
3. Ensure you have [Tesseract OCR](https://tesseract-ocr.github.io/tessdoc/Downloads.html) installed and properly configured.

## Usage

1. Place your financial document images inside the archive folder, organized by document type.
2. Run the script:
  ```bash
  python main.py
  ```
3. After processing, check the extracted_document_info.csv file for extracted data.
   
## Output

### CSV file containing:
- File names
- True and predicted document labels
- Extracted text details
- Prediction accuracy

### Technologies Used
- Python
- Tesseract OCR
- LayoutLM (via Hugging Face Transformers)
- OpenCV
- Pandas

### Contributing
[Ronak Parmar](https://github.com/ronak-create)

License
This project is licensed under the MIT License.
