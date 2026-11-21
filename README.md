# AI Applications Lab (CONT_26ECP-102 / 26ECP-102)
### Chandigarh University — Academic Session 2026–27

Comprehensive repository containing all official lecture presentations, lab manuals, worksheets, real-world datasets, and the **Publication-Grade Master Examination & Lab Practical Compendium (128 Pages)** for **AI Applications Lab (`CONT_26ECP-102`)** at Chandigarh University.

---

## 🚀 Quick Access Links

| Document | Format | Description | Direct Link |
| :--- | :---: | :--- | :--- |
| **Master Compendium (PDF)** | 📄 PDF | **128-Page** publication-grade reference with KaTeX formulas, architecture diagrams, and syntax-highlighted code | [View Master PDF](AI_Applications_Lab_26ECP_102_Master_Compendium.pdf) · [Direct Download](https://raw.githubusercontent.com/KishanKumar-in/cu-ai-applications-lab/main/AI_Applications_Lab_26ECP_102_Master_Compendium.pdf) |
| **Master Compendium (Markdown)** | 📝 MD | Full 273 KB publication source with complete executable Python implementations | [View Master Markdown](AI_Applications_Lab_26ECP_102_Master_Compendium.md) |
| **LMS Raw Semester Notes** | 📑 MD | Consolidated raw lecture notes and slide extractions (10,024 lines) | [View Semester Master](_COMPLETE_CONT_26ECP-102%20__%20AI%20APPLICATIONS%20LAB_SEMESTER_MASTER.md) |

---

## 📚 Master Compendium Structure (128 Pages)

### **Unit 1: Data Pre-processing, EDA & Supervised Machine Learning**
- **Experiment 1.1:** Data Pre-processing, Pandas (`head`, `info`, `describe`, `loc` vs `iloc`), NumPy (1D/2D arrays, vectorization, variance), and Matplotlib (grids, grouped & stacked bar charts, explode pie charts).
- **Experiment 1.2:** Exploratory Data Analysis on `data.csv` (8 complete codes: loading, descriptive stats, missing values & imputation, correlation matrices, heatmaps, boxplot outlier detection via IQR, and scatter plots).
- **Experiment 1.3:** Supervised Classification on `heart.csv.csv` (15 complete codes: data cleaning, stratified train-test split, `StandardScaler` pipeline, Gaussian Naive Bayes, Stratified 5-Fold Cross-Validation, confusion matrix, and ROC-AUC curve).
- **Experiment 1.4:** Comparative Multi-Model Benchmark (Logistic Regression, SVC Linear/RBF, Decision Tree, Random Forest, KNN, Gaussian Naive Bayes, multi-metric comparison table, confusion matrix grid, and cross-validation boxplots).
- **Unit 1 Academic Support:** 10 Viva Voce questions with examiner follow-ups, debugging checklist, and formula cheat sheet.

### **Unit 2: AI Fundamentals, Generative AI, Transformers & Azure AI**
- **Experiment 2.1:** AI Taxonomy (ANI, AGI, ASI), Discriminative vs Generative AI ($P(Y|X)$ vs $P(X,Y)$, Bayes' theorem proof), LLMs vs SLMs parameter scaling ($M = P 	imes B$ for FP16, INT8, INT4), 4-pillar Autonomous Agent architecture (Perception, Planning, Memory, Action), and Azure Machine Learning vs Azure OpenAI architecture.
- **Experiment 2.2:** Evolution from RNNs/LSTMs to Transformers, full Encoder-Decoder stack, Sinusoidal Positional Encoding, Scaled Dot-Product Attention derivation ($rac{QK^T}{\sqrt{d_k}}$ stabilization), Subword Tokenization (BPE, WordPiece, SentencePiece), Word2Vec, GloVe, Cosine similarity, and Adaptation strategies (Prompting vs RAG vs LoRA $\Delta W = BA$).
- **Experiment 2.3:** Full NLP Text Processing Pipeline (Normalization, Tokenization, Stopwords, Stemming vs Lemmatization, POS tagging, NER), executable NLTK + SpaCy pipeline, TF-IDF mathematical derivation, Sentiment Analysis (VADER, TextBlob, Scikit-Learn), and Azure AI Language Text Analytics SDK.
- **Experiment 2.4:** Azure OpenAI Studio & Azure AI Foundry, prompt engineering mechanics, Temperature and Top-p sampling, Prompt Flow DAG orchestration, complete Azure OpenAI Python SDK programs (chat completions + JSON mode with schema validation), token budgeting, and cost/latency formulas.
- **Unit 2 Academic Support:** 10 Viva Voce questions with examiner follow-ups, debugging checklist, and formula sheet.

### **Unit 3: Speech Processing, Computer Vision, OCR & Document Intelligence**
- **Experiment 3.1:** Speech AI, STT, TTS, Audio capture, Nyquist-Shannon sampling theorem ($f_s > 2f_{\max}$), Framing, Windowing (Hamming/Hann), FFT, Mel filter banks, MFCC derivation, Acoustic/Language modeling, Azure AI Speech SDK (`azure_speech_demo.py`), and Librosa feature extraction (`audio_features.py`).
- **Experiment 3.2:** Computer Vision, Digital image representation (RGB, Grayscale, HSV), Filtering, Sobel/Canny edge detection, CNN architecture (2D convolution, stride, padding, pooling, ReLU, softmax), Vision Transformers (ViT) vs CNNs, OpenCV image processing (`image_processing.py`), DeepFace facial analysis (`deepface_analysis.py`), and Azure AI Vision 4.0 (`azure_vision.py`).
- **Experiment 3.3:** Information Extraction (IE) across scanned PDFs/invoices, OCR pipeline (Binarization, Deskewing, Line segmentation, Character recognition), Raw OCR vs Intelligent Document Processing (IDP), Bounding boxes, Azure AI Document Intelligence (`azure_document_intelligence.py`), and Local OCR using OpenCV and Tesseract (`local_ocr.py`).

### **Section 4: Ten High-Yield Solved Lab Practical Programs**
1. End-to-end Data Preprocessing & IQR Outlier Treatment
2. Comprehensive EDA with Heatmaps and Correlation Analysis
3. Supervised Classification Pipeline with Feature Scaling
4. Comparative Multi-Model Benchmark with 5-Fold Stratified CV
5. Tokenization, Stemming, and Lemmatization Pipeline (NLTK)
6. Named Entity Recognition and Dependency Parsing (spaCy)
7. TF-IDF Matrix Computation and Cosine Similarity Matching
8. Audio Feature Extraction (MFCCs & Spectrograms) with Librosa
9. CNN Feature Extraction / DeepFace Facial Emotion Analysis
10. Document OCR & Information Extraction with Bounding Boxes

### **Section 5 to 9: Master Examination Preparation**
- **Section 5:** Comprehensive Master Viva Voce Question Bank (30 questions spanning all 3 Units with detailed model answers and examiner follow-ups).
- **Section 6:** Master Examiner's Pitfalls & Debugging Checklist (15 common errors, causes, and fixes).
- **Section 7:** Ultimate Revision Cheat Sheet (Statistics, Preprocessing, ML Metrics, Transformer Formulas, Audio/Vision Formulas, OCR, Scikit-Learn snippets, and Azure environment variables).
- **Section 8:** Master Practical Exam Preparation Checklist.
- **Section 9:** Final Course Completion Matrix.

---

## 📁 Repository Directory Overview
- `Course Overview/`: Zero lecture slides, course syllabus, and master introductory guidelines.
- `Course Overview/Experiment-1.1/` to `Experiment-3.3/`: Individual experiment folders containing slide decks (`.pptx`), worksheets (`.docx`), datasets (`data.csv`, `heart.csv.csv`), and extracted lecture text (`.md`).
- `AI_Applications_Lab_26ECP_102_Master_Compendium.pdf`: Complete 128-page compiled master PDF.
- `AI_Applications_Lab_26ECP_102_Master_Compendium.md`: Complete 273 KB master markdown compendium.
- `_COMPLETE_CONT_26ECP-102 __ AI APPLICATIONS LAB_SEMESTER_MASTER.md`: Master consolidated markdown compendium (314 KB, 10,024 lines).

---

## 📖 Recommended References & Textbooks
- **T1:** *Data Science from Scratch*, Joel Grus (O'Reilly).
- **T2:** *Artificial Intelligence: A Modern Approach*, Stuart Russell & Peter Norvig (Pearson).
- **T3:** *Machine Learning*, Tom Mitchell (McGraw Hill).
- **T4:** *Microsoft Azure Fundamentals AZ-900 Exam Ref*, Jim Cheshire & Michael Collier (Microsoft Press).
- **RB1:** *Introduction to Machine Learning with Python*, Andreas C. Müller & Sarah Guido (O'Reilly).
