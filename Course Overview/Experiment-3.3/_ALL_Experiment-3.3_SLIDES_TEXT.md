# Experiment-3.3 - All Lecture Slides Text


## Exp 3.3
### Slide 1
- UNIVERSITY INSTITUTE OF
- ENGINEERING
- DEPARTMENT OF ENGINEERING FOUNDATION-2
- PROGRAM
- NAME
- :
- Bachelor
- of Engineering
- SPECIALIZATION
- :
- COMPUTER SCIENCE & ENGINEERING
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 3                   Experiment No.3.3
- Topic
- : Understanding Vision AI and Information Extraction Workflows with Microsoft Foundry
- Tools
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning
- Objectives
- After
- completing this experiment, students will be able
- to:
- Understand information extraction in
- AI
- Study
- OCR and its working
- Learn
- field extraction and
- mapping
- Understand
- normalization and validation
- Explore real-world
- applications

### Slide 3
- Recap
- of Previous Experiment
- Computer vision is a branch of Artificial Intelligence that helps machines understand images, videos, and camera inputs.
- Images are represented using pixels, gray scale values, and RGB color channels.
- Image processing uses filters, kernels, and convolution to improve images and extract important features.
- Major computer vision tasks include image classification, object detection, semantic segmentation, and contextual image analysis.
- CNNs and Vision Transformers are used to learn visual features and recognize patterns in images.

### Slide 4
- Figure-1 :
- OCR and Translation Pipeline
- Source
- :
- https://medium.com/towards-applied-generative-
- ai
- /moving-on-to-vlms-from-ocr-though-not-totally-649f32aa0729
- Topic(s
- )
- Introduction to Information Extraction
- Optical Character Recognition
- OCR Pipeline
- Field Extraction and Field Mapping
- Information Extraction and OCR Pipeline in AI

### Slide 5
- Figure-2:
- Information
- Extraction
- Source:
- https
- ://www.researchgate.net/publication/220135843_A_strategy_for_extracting_information_from_semi-structured_web_pages/figures
- Information extraction is an AI technique used to convert
- unstructured data into structured data
- Works on documents like invoices, receipts, contracts, and forms
- Example:
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Invoice → Vendor name, date, total
- amount
- Benefits:
- Reduces manual effort
- Saves time
- Improves accuracy
- Enables automation
- Information Extraction

### Slide 6
- OCR converts
- image-based text into machine-readable text
- Works on scanned documents, PDFs, screenshots, and photos
- Uses:
- Receipt scanning
- Form processing
- Business card reading
- Important Point:
- </a:r><a:br><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Higher image quality → Better OCR accuracy
- Figure-3
- : Optical Character Recognition (OCR)
- Source:
- https
- ://www.globe3.com/news/ocr-integration-in-erp/
- Optical Character Recognition (OCR)

### Slide 7
- OCR works in multiple stages
- :
- Image acquisition (input image)
- Pre-processing
- (improve quality)
- Text detection (locate text regions)
- Character recognition (identify text)
- Output generation (digital text)
- This
- pipeline converts images into usable text data
- Figure-4
- :OCR Pipeline
- Source:
- https
- ://theailearner.com/2019/05/28/optical-character-recognition-pipeline/
- OCR Pipeline

### Slide 8
- Preprocessing:
- Removes noise and improves contrast
- Corrects tilted images
- Text Detection:
- Identifies areas containing text
- Separates text from
- images/logos
- Recognition:
- Uses AI models to read characters
- Post-processing:
- Corrects errors and formats output
- Figure-5
- :Key OCR Stages
- Source:
- https
- ://www.highradius.com/resources/Blog/3-steps-to-measuring-effectiveness-of-ocr-and-cash-application-automation/
- Key OCR Stages

### Slide 9
- Field extraction converts OCR text into
- meaningful structured data
- Example:
- Raw Text:
- Date: 15/08/2024
- Structured Field:
- Date →
- 2024-08-15
- Helps systems understand and use extracted data
- Figure-6
- : Field Extraction
- Source:
- https
- ://www.geeksforgeeks.org/nlp/information-extraction-in-nlp/
- Field Extraction

### Slide 10
- Figure-7 :
- OCR
- vs
- Field Extraction
- Source:
- https
- ://parseur.com/blog/
- ocr
- -
- vs
- -document-processing
- OCR
- vs
- Field Extraction
- OCR
- Field Extraction
- Reads text
- Understands meaning
- Output = raw text
- Output = structured data
- Example:
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>₹5000 →
- OCR: value
- Field Extraction: total
- amount
- Both
- are required for complete document processing

### Slide 11
- Steps involved:
- OCR output ingestion
- Field detection (find useful values)
- Field mapping (assign labels)
- Data normalization (standard format)
- Validation (check correctness)
- Integration with systems
- Converts
- raw text into business-ready data
- Figure-8 :
- PDF Data
- Extraction
- Source:
- https
- ://www.docupipe.ai/blog/pdf-data-extraction
- Field Extraction Pipeline

### Slide 12
- Summary of the
- Experiment
- Information extraction is an AI technique that converts unstructured data (documents, images) into structured and usable data fields for automation
- .
- OCR plays a key role by extracting text from images and documents, forming the foundation for further data processing.
- Field extraction and mapping help in understanding the meaning of extracted text and organizing it into structured formats like names, dates, and amounts.
- The complete pipeline includes OCR, detection, mapping, normalization, and validation, ensuring accurate and reliable data extraction.

### Slide 13
- Quiz/ FAQ’s
- What is information extraction in artificial intelligence?
- What
- type of data is converted into structured form using information extraction?
- What
- is the full form of OCR?
- What
- is the main purpose of Optical Character Recognition?
- Name
- any two stages of the OCR pipeline.
- What
- is preprocessing in OCR? Why is it important?
- What
- is field extraction? What is the difference between OCR and field extraction?

### Slide 14
- R
- eferences/ Articles/ Videos
- References / Articles
- Microsoft Learn – Introduction to Document Intelligence
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId3"/></a:rPr><a:t>https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/overview
- Microsoft
- Learn – Optical Character Recognition (OCR)
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/overview-ocr
- IBM
- – What is Optical Character
- Recognition?
- https://www.ibm.com/topics/ocr
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t/></a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" b="1" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Videos
- What is OCR? | Optical Character Recognition
- Explained
- https://www.youtube.com/watch?v=5qg4j8zqZ3k
- </a:r><a:br><a:rPr lang="en-IN" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1600" b="1" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>AI
- Explained | Intelligent Document
- Processing
- https://www.youtube.com/watch?v=Gm8Qd9Xv7hY
- </a:r><a:br><a:rPr lang="en-IN" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1600" b="1" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>OCR
- Tutorial using Python and
- Tesseract
- </a:r><a:br><a:rPr lang="en-IN" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1600" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId8"/></a:rPr><a:t>https://www.youtube.com/watch?v=Hj1d9T9UQ9Q

### Slide 15
- Additional
- learning
- R
- esources
- TensorFlow
- – Image and Document Processing Tutorials
- </a:r><a:br><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId3"/></a:rPr><a:t>https://
- www.tensorflow.org/tutorials
- PyTorch
- – Computer Vision and OCR Tutorials
- </a:r><a:br><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://pytorch.org/tutorials/
- Hugging
- Face – Document AI and NLP Course
- </a:r><a:br><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId5"/></a:rPr><a:t>https://huggingface.co/learn
- OpenCV
- Documentation – Image Processing and OCR Basics
- </a:r><a:br><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId6"/></a:rPr><a:t>https://docs.opencv.org/

### Slide 16
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 17
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in
