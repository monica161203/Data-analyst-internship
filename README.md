# 🧾 Intelligent Text Extraction from Invoices using OCR & AWS Textract

This project was developed during my **Data Analyst Internship at MindGeniX** (June 4 – July 4, 2025) under the mentorship of **Mr. Vijayakumar Muniyandi**. The objective was to extract structured data—especially tables and key-value fields—from scanned and digital hospital invoices in PDF/image formats using a combination of OCR techniques and cloud-based solutions.

## 🚀 Project Goal

To build a robust and automated pipeline that:
- Accurately extracts text and tables from scanned/digital documents
- Handles layout variations across different invoices
- Converts unstructured text into structured formats like CSV, Excel, or JSON

## 🧪 Tools & Technologies

- **Python 3.10**
- **EasyOCR** – For initial text extraction trials
- **Tabula-py** – Java-based tool for table extraction from PDFs
- **Camelot** – Lightweight PDF table extractor
- **AWS Textract** – Cloud-based OCR for text, forms, and tables
- **AWS S3** – Storage and API access for Textract
- **Boto3** – Python SDK for AWS
- **Pandas** – Data structuring and export

## 🔁 Workflow Overview

1. **EasyOCR**:
   - Performed basic OCR on PDFs/images
   - Lacked table recognition and formatting

2. **Tabula & Camelot**:
   - Tested on digital PDFs
   - Worked well for clean layouts, failed on scanned documents

3. **AWS Textract Integration**:
   - Uploaded files to S3 bucket
   - Triggered Textract via Python API
   - Extracted text, key-value pairs, and tables accurately
   - Parsed responses and stored in structured formats


## ✅ Results

- AWS Textract provided the **most accurate** and **structured extraction**, especially for scanned documents
- Clean conversion of key-value data and tables to **CSV, Excel, and JSON**
- Developed a reusable Python workflow for document processing

## 📈 Key Learnings

- Every OCR tool has strengths and limitations depending on the document type
- Table extraction is far more complex than plain text OCR
- Cloud-based APIs like **AWS Textract** simplify and scale document processing tasks
- Real-world problems require **iteration, testing, and flexibility**

