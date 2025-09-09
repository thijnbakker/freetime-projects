# Image Processing Pipelines

This repository contains two Jupyter notebooks implementing full image-to-CSV pipelines for bar‐chart images:

- **`pipeline_image_1.ipynb`**  
  Processes `dataset_part2/image_1.png`.  
  1. Loads and crops the image with OpenCV.  
  2. Applies K-means clustering to segment bars.  
  3. Uses EasyOCR and Tesseract OCR to extract axis labels.  
  4. Cleans and groups text via NLTK’s WordNet (common category extraction).  
  5. Exports the results as a CSV and prints a pandas DataFrame summary.

- **`pipeline_image_2.ipynb`**  
  Same steps as above, for `dataset_part2/image_2.png`.

## Prerequisites

1. **Python 3.7+**  
2. **Tesseract-OCR**  
   - Install the Tesseract engine for your OS.  
   - On Windows, update the path in each notebook’s  
     ```python
     pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'
     ```
     to match your installation directory.

3. **NLTK Data**  
   ```bash
   python -c "import nltk; nltk.download('wordnet')"
