# Experiment-3.3

##

## Understanding Vision AI and Information Extraction workflows with Microsoft Foundry Tools.

##

## CO5

##

## Aim

To study AI-based information extraction and understand how structured data can be extracted from unstructured documents and images using OCR, field extraction, field mapping, and data normalization techniques.

## Objectives

- To understand the concept of information extraction in artificial intelligence.

- To study the role of OCR in converting image-based text into machine-readable text.

- To understand field extraction and field mapping.

- To learn how extracted data is normalized, validated, and used in business systems.

- To study applications of information extraction in finance, healthcare, legal, logistics, and business automation.

## Theory

## Introduction to Information Extraction

Information extraction is an important application of artificial intelligence that is used to extract useful and meaningful data from unstructured or semi-structured content, as shown in Figure 1. Unstructured data may be present in scanned documents, images, receipts, invoices, contracts, medical records, business cards, and forms.

AI-based information extraction converts this unstructured data into structured data fields. For example, from an invoice, AI can extract vendor name, invoice number, date, tax amount, payment terms, product details, and total amount. This extracted information can then be stored in a database, spreadsheet, or business application.

The main purpose of information extraction is to reduce manual work, save time, improve accuracy, and support automation in document-based processes.

## Figure 1: Types of information extraction from text, image, audio, and video data.

## Need for Information Extraction

Many organizations process a large number of documents every day. Manual processing of these documents is slow, costly, and may contain human errors. Information extraction helps solve this problem by automatically reading documents and extracting important information.

For example, in finance, it can be used to process invoices and receipts. In healthcare, it can extract patient details and medical information. In logistics, it can extract shipment numbers, addresses, and delivery details. Therefore, information extraction is useful for digital transformation and business workflow automation.

## Working Concept of Information Extraction

AI-based information extraction generally works in two main stages. The first stage is text extraction, and the second stage is field extraction.

In text extraction, the system reads text from documents or images using Optical Character Recognition, also called OCR. In field extraction, the system understands the meaning of the extracted text and maps it to proper data fields.

For example, OCR may extract the text “Invoice No: 12345.” Field extraction identifies “12345” as the invoice number. Similarly, “Total: ₹5000” is mapped as the total amount.

## Optical Character Recognition

Optical Character Recognition, or OCR, is a technology that converts visual text into editable and searchable digital text. Visual text may be present in scanned documents, images, PDFs, screenshots, handwritten forms, receipts, and business cards as shown in Figure 2.

OCR is an important part of information extraction because the accuracy of field extraction depends on the quality of OCR output. If OCR extracts incorrect text, the final extracted fields may also be incorrect.

## Figure 2: Optical Character Recognition for converting images, PDFs, and scanned documents into editable text.

## OCR Pipeline

The OCR pipeline consists of the following stages:

- Image acquisition and input

- Preprocessing and image enhancement

- Text region detection

- Character recognition and classification

- Output generation and post-processing

These stages work together to convert image-based text into usable digital text, as shown in Figure 3.

## Figure 3: OCR workflow for extracting text from an input image.

##

## Image Acquisition and Input

Image acquisition is the first stage of OCR. In this stage, the system receives an input image or document containing text. The input may be a scanned document, mobile photograph, screenshot, PDF page, or video frame.

The quality of the input image is very important. Clear, properly aligned, and high-resolution images give better OCR results, while blurred, tilted, or low-light images may reduce accuracy.

## Preprocessing and Image Enhancement

Preprocessing is used to improve the quality of the input image before text recognition. It helps the OCR system read the text more clearly.

Important preprocessing techniques include noise reduction, contrast adjustment, skew correction, and resolution optimization. Noise reduction removes unwanted marks and dust. Contrast adjustment makes the text more visible. Skew correction straightens tilted documents. Resolution optimization improves low-quality images.

Good preprocessing improves OCR accuracy.

## Text Region Detection

Text region detection is the stage where the system identifies areas of the document that contain text. A document may contain text, images, logos, signatures, tables, stamps, and blank spaces. The OCR system must separate text regions from non-text areas.

This stage also identifies headings, paragraphs, captions, table text, and reading order. Correct reading order is important because the wrong order can change the meaning of the extracted text.

## Character Recognition and Classification

Character recognition is the main stage of OCR. In this stage, the system recognizes letters, numbers, and symbols from the detected text regions.

The system analyzes the shape and pattern of each character and identifies it using trained models. Modern OCR systems use machine learning and deep learning models such as CNNs and transformers. These models can recognize text more accurately even when fonts, sizes, or layouts are different.

Context analysis may also be used to correct mistakes. For example, if OCR reads “Invo1ce,” the system may correct it as “Invoice.”

## Output Generation and Post-Processing

After recognizing the characters, the OCR system generates digital text output. This output may include words, sentences, paragraphs, line breaks, tables, and layout details.

Post-processing improves the final result by applying spelling correction, grammar checking, formatting, confidence scoring, and structure preservation. Confidence scores show how certain the system is about the recognized text.

## Field Extraction

Field extraction is the process of identifying meaningful data fields from OCR output. OCR only tells what text is present, but field extraction tells what the text means.

For example, OCR may extract:

Fourth Coffee

2024-08-15

Subtotal: $6.48

Tax: $0.49

Total: $6.97

Field extraction identifies these as:

Vendor: Fourth Coffee

Date: 2024-08-15

Subtotal: $6.48

Tax: $0.49

Total: $6.97

Thus, field extraction converts raw OCR text into labeled and structured information.

## Difference Between OCR and Field Extraction

OCR and field extraction are connected but different. OCR extracts text from images or documents, while field extraction gives meaning to that text.

For example, OCR may detect the value “₹10,500.” Field extraction identifies whether it is the total amount, tax amount, unit price, or balance amount. Therefore, OCR reads the text, and field extraction understands the text.

## Field Extraction Pipeline

The field extraction pipeline includes:

- OCR output ingestion

- Field detection and candidate identification

- Field mapping and association

- Data normalization and standardization

- Integration with business systems

These steps help convert raw OCR output into useful structured data, as shown in Figure 3.

## Figure 3: Intelligent document processing pipeline for document classification, data extraction, validation, and integration.

## OCR Output Ingestion

OCR output ingestion means taking the text extracted by OCR as input for field extraction. This output may include raw text, text position, confidence scores, page number, layout information, and reading order.

The position of text is very important. For example, a number near the label “Invoice Number” is likely to be an invoice number, while a number near “Total” is likely to be the total amount.

## Field Detection and Candidate Identification

Field detection identifies possible field values from OCR output. A document may contain many names, dates, numbers, and amounts. The system must identify which values are useful.

There are three common approaches:

Template-based detection uses fixed rules and known document layouts. It works well for standard forms.

Machine learning-based detection uses trained models to identify fields from different document formats.

Generative AI-based extraction uses large language models to extract fields according to a given schema, such as vendor name, date, invoice number, and total amount.

## Field Mapping and Association

Field mapping connects extracted values with correct field names. For example, it maps “Fourth Coffee” to vendor name and “$6.97” to total amount.

Field mapping may use proximity analysis, key-value pairing, reading order, named entity recognition, and table processing. Proximity analysis checks how close a value is to its label. Key-value pairing identifies pairs such as “Name: Rachit” or “Date: 15-08-2024.”

## Table and Structured Content Extraction

Many documents contain tables, especially invoices and receipts. These tables may include item names, quantities, unit prices, tax, discounts, and totals.

Table extraction identifies rows, columns, headers, and cell values. It helps map table data correctly. For example, in an invoice table, each row may represent one product, and each column may represent item description, quantity, price, and total.

## Confidence Scoring and Validation

Confidence scoring shows how reliable the extracted text or field value is. A high confidence score means the system is more certain about the result. A low confidence score may require human review.

Validation checks whether the extracted data is correct. For example, in an invoice, the system can check whether item totals and tax match the final total. This improves the accuracy and reliability of information extraction.

## Data Normalization and Standardization

Data normalization converts extracted values into a common and standard format.

For example, dates such as 15/08/2024, 08-15-2024, and August 15, 2024 can be converted into a standard format like 2024-08-15. Currency values such as ₹5,000 and Rs. 5000 can also be standardized.

Text standardization may include correcting capitalization, removing extra spaces, and expanding abbreviations.

## Integration with Business Systems

After extraction, mapping, validation, and normalization, the structured data can be sent to business systems such as databases, accounting software, ERP systems, hospital management systems, or workflow automation tools.

For example, invoice data can be sent to accounting software, patient information can be sent to hospital systems, and shipment data can be sent to logistics tracking systems.

## Applications of Information Extraction

Information extraction is used in many areas. In finance, it is used for invoice processing, receipt scanning, expense claims, and bank statement analysis. In legal work, it is used for contract processing and compliance documents. In healthcare, it is used to extract patient details, diagnosis, medication lists, and billing codes.

It is also used in logistics for shipping documents, purchase orders, tracking numbers, customs forms, and delivery instructions. Business card scanning is another common application where name, company, phone number, email, and job title are extracted.

## Code

# 1. Install OCR tools

!apt-get -qq install tesseract-ocr > /dev/null

!pip -q install pytesseract

# 2. Import libraries

import pytesseract

from PIL import Image, ImageOps

from google.colab import files

from IPython.display import display

# 3. Upload an image

print("Upload an image containing printed English text:")

uploaded = files.upload()

if uploaded:

filename = next(iter(uploaded))

# 4. Open and display the image

image = ImageOps.exif_transpose(Image.open(filename))

display(image)

# 5. Convert to grayscale and extract text

gray_image = ImageOps.grayscale(image)

text = pytesseract.image_to_string(gray_image, lang="eng")

# 6. Display extracted text

print("\nEXTRACTED TEXT:\n")

print(text.strip() or "No text detected. Try a clearer image.")

## Practice Task Questions

- Take a sample invoice image and identify the fields that can be extracted from it, such as invoice number, date, vendor name, tax amount, and total amount.

- Collect a receipt image and list the information that an AI system can extract from it, such as merchant name, purchased items, price, tax, and payment method.

- Take a business card image and identify the structured fields such as name, designation, company name, phone number, email address, and website.

- Prepare a sample scanned document and explain how OCR can convert the text present in the image into editable digital text.

- Take any form or application document and mark the key-value pairs present in it, such as name, address, date of birth, ID number, and contact number.

- Compare a clear document image and a blurred document image, and write how image quality affects OCR accuracy.

- Create a small table showing the difference between OCR and field extraction using any one example document.

- Take an invoice containing line items and identify the table fields such as item name, quantity, unit price, tax, discount, and total.

- Choose any extracted values from a document and normalize them into standard formats, such as date format, currency format, and phone number format.

- Prepare a short report explaining how AI-based information extraction can be used in any one field, such as finance, healthcare, legal documents, logistics, or education.

## Video Links

Azure AI Document Intelligence Hands-On: Analyze, Extract

Azure AI Document Intelligence is awesome! A simple intro.

Introduction to Optical Character Recognition (OCR)

Text detection with Python and OpenCV | OCR using EasyOCR | Computer Vision Tutorial

How to use Document AI

## Additional Resources

- Microsoft Learn: Azure AI Document Intelligence Documentation

Link: https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/

Useful for learning OCR, key-value pair extraction, tables, forms, and document processing using Azure AI.

- Microsoft Learn: Document Intelligence Read OCR Model

Link: https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/prebuilt/read

Useful for understanding how OCR extracts printed and handwritten text from scanned and digital documents.

- Google Cloud: Document AI

Link: https://cloud.google.com/document-ai

Useful for learning document OCR, document classification, layout extraction, and entity extraction.

- Google Cloud: Document AI Extraction Overview

Link: https://docs.cloud.google.com/document-ai/docs/extracting-overview

Useful for understanding custom field extraction, schema-based extraction, and document entity extraction.

- Google Cloud: Enterprise Document OCR

Link: https://docs.cloud.google.com/document-ai/docs/enterprise-document-ocr

Useful for learning how OCR detects text and layout information from different document types.

- AWS: Amazon Textract

Link: https://aws.amazon.com/textract/

Useful for learning automatic extraction of text, handwriting, layout elements, tables, and forms from scanned documents.

- AWS Documentation: Amazon Textract Tables

Link: https://docs.aws.amazon.com/textract/latest/dg/how-it-works-tables.html

Useful for understanding how tables are detected and extracted from documents.

- IBM: What is Intelligent Document Processing?

Link: https://www.ibm.com/think/topics/intelligent-document-processing

Useful for understanding how AI extracts business-critical data from documents for faster decision-making.

- IBM watsonx: Understanding Documents

Link: https://www.ibm.com/docs/en/watsonx/saas?topic=generation-understanding-documents

Useful for learning key-value pair classification and extraction from structured and domain-specific documents.

- IBM watsonx: Text Extraction

Link: https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-api-text-extraction.html?context=wx

Useful for understanding OCR-based text extraction from scanned PDFs and images.

## Textbooks

- Speech and Language Processing — Daniel Jurafsky and James H. Martin

PDF/Online Link: https://web.stanford.edu/~jurafsky/slp3/

- Introduction to Information Retrieval — Christopher D. Manning, Prabhakar Raghavan, Hinrich Schütze

PDF Link: https://nlp.stanford.edu/IR-book/pdf/irbookonlinereading.pdf

- Computer Vision: Algorithms and Applications — Richard Szeliski

PDF/Online Link: https://szeliski.org/Book/

- Dive into Deep Learning—Aston Zhang, Zachary C. Lipton, Mu Li, Alexander J. Smola

PDF Link: https://d2l.ai/d2l-en.pdf

- Artificial Intelligence: Foundations of Computational Agents — David L. Poole and Alan K. Mackworth

Online Book Link: https://artint.info/3e/html/ArtInt3e.html

## Reference Books / Reference Materials

- Optical Character Recognition—Line Eikvil

PDF Link: https://home.nr.no/~eikvil/OCR.pdf

- OCR — Optical Character Recognition Technology — United Nations Statistics Division

PDF Link: https://unstats.un.org/unsd/demographic/sources/census/wphc/dataCapture/docs/Data-Capture_ch06-ABS.pdf

- Natural Language Processing for Information Extraction — Sonit Singh

PDF Link: https://arxiv.org/pdf/1807.02383

- Open Information Extraction — Duc-Thuan Vo and Ebrahim Bagheri

PDF Link: https://arxiv.org/pdf/1607.02784

- LexNLP: Natural Language Processing and Information Extraction for Legal and Regulatory Texts — Michael J. Bommarito II, Daniel Martin Katz, Eric M. Detterman

PDF Link: https://arxiv.org/pdf/1806.03688