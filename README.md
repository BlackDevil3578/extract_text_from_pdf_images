## PDF to Text Conversion with OCR and Image Processing

### Description

This project provides an effective solution for extracting text from PDF files where each page is an image. The script extracts high-resolution images from PDF pages , preprocesses these images to enhance quality, and uses Tesseract OCR to extract text. The extracted text is then saved to a text file.

### Features

- **High-Resolution Image Extraction**: Converts PDF pages to high-resolution images to improve OCR accuracy.
- **Advanced Image Processing**: Applies grayscale conversion, contrast adjustment, and noise reduction to enhance image quality.
- **OCR with Tesseract**: Extracts text from images using Tesseract OCR with support for multiple languages.
- **Automated Workflow**: Processes all images in a folder and extracts text, saving it to a single text file.

### Dependencies

- `PyMuPDF` (`fitz`): For converting PDF pages to images.
- `Pillow` (`PIL`): For image manipulation and preprocessing.
- `OpenCV` (`cv2`): For additional image processing.
- `pytesseract`: For OCR text extraction.
- `numpy`: For handling image data arrays.

### Installation

1. Install Python (3.6+ recommended).
2. Install the required packages:
    ```sh
    pip install pymupdf pillow opencv-python pytesseract numpy
    ```
3. Install Tesseract OCR and ensure it is available in your system PATH. Update the `pytesseract.pytesseract.tesseract_cmd` variable in the script to point to your Tesseract executable if necessary.

### Usage

1. Place your PDF file in the working directory.
2. Run the script and input the PDF file path when prompted:
    ```sh
    python script.py
    ```

### Example

```python
pdf_path = "path/to/your/document.pdf"
pdf_to_text(pdf_path, zoom_factor=8.0)
"# extract_text_from_pdf_images" 
