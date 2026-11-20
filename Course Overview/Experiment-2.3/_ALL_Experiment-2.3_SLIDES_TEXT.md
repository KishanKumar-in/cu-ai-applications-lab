# Experiment-2.3 - All Lecture Slides Text


## Exp 2.3
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
- Unit No. 2                   Experiment No.2.3
- Topic
- : Exploring Generative AI, Natural Language Processing and Azure
- AI
- Tools.
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
- To understand the role of text analysis in Artificial Intelligence and Natural Language Processing
- .
- To
- learn how unstructured text is converted into meaningful and structured information
- .
- To
- understand tokenization and different text preprocessing techniques
- .
- To
- study statistical text analysis methods such as frequency analysis, Bag-of-Words, and TF-IDF
- .
- To
- understand semantic language models, word
- embedding's,
- and cosine similarity.

### Slide 3
- Recap
- of Previous Experiment
- Generative AI can create new content such as text, images, audio, video, and code.
- Prompts are inputs given to AI models, and better prompts produce better responses.
- Large Language Models process language using tokens, embedding's, transformers, and attention mechanisms.
- Retrieval Augmented Generation improves AI responses by retrieving relevant external information.

### Slide 4
- Topic 1:
- Introduction to Text
- Analysis
- Topic 2:
- Tokenization and Text
- Preprocessing
- Topic 3:
- Statistical Text
- Analysis
- Topic 4:
- Semantic Language Models
- Figure-1 :
- Text Analysis using NLP
- Source :
- https://pagadala-saiteja.medium.com/an-introduction-to-natural-language-processing-for-text-analysis-7856267266d5
- Text Analysis using NLP

### Slide 5
- Figure-2:
- Text analysis Techniques
- Source:
- https
- ://
- forms.app
- /en/blog/text-analysis
- Introduction to Text Analysis
- Text analysis is a subset of
- Natural Language Processing
- that enables machines to extract meaning, structure, and useful insights from unstructured text
- .
- Text analysis helps convert raw text into actionable information for decision-making
- .
- Common use cases include:
- Language detection
- Key term extraction
- Entity detection
- PII detection
- Text classification
- Sentiment analysis
- Text summarization

### Slide 6
- Tokenization is the first step in text analysis.
- It is the process of breaking a sentence, paragraph, or document into smaller units called
- tokens
- .
- Example
- :
- </a:r><a:br><a:rPr lang="en-US" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Sentence: “We choose to go to the moon”
- Tokens:
- </a:r><a:br><a:rPr lang="en-US" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>We
- choose
- to
- go
- to
- the
- moon
- Figure-3
- :Tokenization in
- NLP
- Source:
- https
- ://www.geeksforgeeks.org/nlp/nlp-how-tokenizing-text-sentence-words-works/
- Tokenization

### Slide 7
- Common
- preprocessing techniques include:
- Text Normalization:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Converting text into lowercase and removing punctuation or special symbols.
- Stop Word Removal:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Removing common words such as “the”, “is”, “a”, “an”, and “of”.
- N-Gram Extraction:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Finding word groups such as “artificial intelligence” or “natural language processing”.
- Stemming:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Reducing words to their root form by removing endings.
- Lemmatization:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Converting words into their valid dictionary form.
- POS Tagging:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Identifying grammatical roles such as noun, verb, adjective, or adverb.
- Figure-4
- :Text Pre-processing Techniques
- Source:
- https
- ://www.linkedin.com/pulse/unlocking-power-text-deep-dive-nlp-its-preprocessing-dr-hesam-akhtar-rkgsc/
- Text
- Pre-processing
- Techniques

### Slide 8
- After tokenization and preprocessing, statistical techniques are used to identify patterns and meaning from text.
- Frequency Analysis:
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Counts how many times each word appears in a document.
- Frequently
- occurring words often indicate the main topic of the document.
- Bag-of-Words:
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Represents text as word counts or word occurrences.
- It ignores grammar and word order but is useful for machine learning tasks.
- TF-IDF:
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Term Frequency-Inverse Document Frequency identifies important words in a document compared with other documents.
- A high TF-IDF score means a word is important in one document but not common in all documents.
- Figure-5
- :Statistical Text Analysis
- Source:
- https
- ://loganix.com/what-is-
- tf
- -
- idf
- /
- Statistical Text Analysis

### Slide 9
- Bag-of-Words Model
- Bag-of-Words converts text into numerical form by counting word occurrences.
- It is commonly used in:
- Spam detection
- Sentiment analysis
- Text classification
- Document
- categorization
- TF-IDF
- TF-IDF gives importance to words that appear frequently in one document but rarely across other documents.
- Formula:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>TF-IDF = Term Frequency × Inverse Document Frequency
- TF-IDF is useful for keyword extraction and document comparison.
- Figure-6
- :
- Bag-of-Words
- Source:
- https
- ://ayselaydin.medium.com/4-bag-of-words-model-in-nlp-434cb38cdd1b
- Bag-of-Words and TF-IDF

### Slide 10
- Text Rank
- Text Rank
- is an unsupervised graph-based algorithm used for text summarization and keyword extraction
- .
- In Text Rank,
- each sentence is treated as a node in a graph.
- Connections between sentences are created based on similarity
- .
- Steps
- in
- Text Rank:
- Split the document into sentences
- Create sentence nodes
- Calculate similarity between sentences
- Rank the sentences
- Select top-ranked sentences for
- summary
- Figure-7
- :
- Text Rank for Text Summarization
- Source:
- https
- ://www.analyticsvidhya.com/blog/2018/11/introduction-text-summarization-textrank-python/
- Text Rank
- for Text Summarization

### Slide 11
- Word
- Embedding's
- and Cosine Similarity
- Word
- embedding's
- represent words as vectors.
- A vector is a list of numbers that captures the meaning of a word
- .
- Example:
- dog = [0.8, 0.6, 0.1]
- cat = [0.7, 0.5, 0.2]
- tree = [0.2, 0.1, 0.9]
- Cosine similarity is used to measure similarity between two vectors.
- If cosine similarity is close to 1, the words are highly similar.
- If cosine similarity is close to 0, the words are less similar.
- Figure-8
- :
- Word Embedding's and Cosine Similarity
- Source:
- https
- ://www.geeksforgeeks.org/nlp/tokenization-vs-embeddings/
- Word
- Embedding's
- and Cosine Similarity

### Slide 12
- Semantic Language Models
- Semantic language models understand the meaning and context of words
- .
- Modern NLP models represent words as numerical vectors called
- embedding's
- .
- Words with similar meanings have similar vector directions
- .
- Example:
- Dog and cat have similar meanings because both are animals.
- Dog and tree have less similarity because they belong to different categories
- .
- Figure-9:
- Semantic Language Models
- Source:
- https
- ://se-rwth.github.io/research/Semantics/
- Semantic Language Models

### Slide 13
- Summary of the
- Experiment
- Text analysis is an important application of Artificial Intelligence and Natural Language Processing
- .
- Tokenization breaks text into smaller units called tokens
- .
- Frequency analysis, Bag-of-Words, and TF-IDF are statistical techniques for text representation
- .
- Text Rank
- is used for extractive summarization and keyword extraction
- .
- Semantic language models use
- embedding's
- to understand meaning and context
- .
- Text analysis is useful in sentiment analysis, spam detection,
- Chabot's,
- search engines, and summarization.

### Slide 14
- Next
- Experiment
- T
- opic(s)
- Introduction to Speech AI
- Speech-to-Text
- and Automatic Speech
- Recognition
- Text-to-Speech
- and Speech
- Synthesis
- Voice
- Assistants and Real-World Applications

### Slide 15
- Quiz/ FAQ’s
- What is text analysis
- ?
- What
- is tokenization
- ?
- What
- is the difference between stemming and lemmatization
- ?
- What
- are stop words
- ?
- What
- is Bag-of-Words
- ?
- What
- is TF-IDF
- ?
- What
- are word
- embedding's?
- What
- is cosine similarity
- ?

### Slide 16
- R
- eferences/ Articles/ Videos
- Reference / Articles
- Natural Language Processing with Python
- https://www.nltk.org/book/
- Speech and Language Processing
- https://web.stanford.edu/~jurafsky/slp3/
- Scikit
- -learn Text Feature Extraction
- https://
- scikit-learn.org/stable/modules/feature_extraction.html
- Videos
- Natural Language Processing - Tokenization
- https://www.youtube.com/watch?v=O2jGzHSJzpg
- Text Representation using TF-IDF
- https://www.youtube.com/watch?v=ATK6fm3cYfI
- Introduction to NLP Bag-of-Words Model
- https://www.youtube.com/watch?v=8Mlc4-3tgzc

### Slide 17
- Additional
- learning
- R
- esources
- Additional Resources for Learning NLP Basics
- https://www.nltk.org/
- </a:r><a:br><a:rPr lang="en-US" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://www.nltk.org/book/
- Additional Resources for Text Preprocessing
- https://www.geeksforgeeks.org/nlp/text-preprocessing-for-nlp-tasks/
- Additional Resources for Bag-of-Words and TF-IDF
- https://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html
- Additional Resources for Semantic Models
- https://web.stanford.edu/~jurafsky/slp3/

### Slide 18
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 19
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in
