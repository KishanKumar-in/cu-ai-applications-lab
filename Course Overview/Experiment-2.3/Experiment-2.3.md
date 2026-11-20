# Experiment-2.3

## Exploring Generative AI , Natural Language Processing, and Azure AI tools.

##      CO4

##

## Aim

To study and implement the basic concepts of Text Analysis using Natural Language Processing, including tokenization, text normalization, stop word removal, stemming, lemmatization, POS tagging, frequency analysis, TF-IDF, bag-of-words, TextRank, and semantic language models.

## Objectives

The objectives of this experiment are:

- To understand the meaning and importance of text analysis in Artificial Intelligence.

- To learn how unstructured text is converted into meaningful structured information.

- To perform tokenization on a given text corpus.

- To apply text preprocessing techniques such as normalization, stop word removal, stemming, and lemmatization.

- To understand statistical text analysis using frequency analysis and TF-IDF.

- To understand bag-of-words representation for machine learning.

- To study TextRank for text summarization and keyword extraction.

- To understand semantic language models, embeddings, and cosine similarity.

- To identify real-world applications of NLP-based text analysis.

## Theory

## Introduction to Text Analysis

Text analysis is a part of Natural Language Processing, also called NLP. NLP is a branch of Artificial Intelligence that helps computers understand, process, and analyze human language as shown in Figure 1.

Figure 1: Common NLP tasks, including speech recognition, speech tagging, word sense disambiguation, named entity recognition, coreference resolution, and natural language generation.

Most real-world data is available in unstructured form, such as emails, reviews, social media posts, contracts, news articles, support tickets, and documents. Since this data is not arranged in rows and columns like a database, computers cannot directly understand it. Text analysis helps convert this unstructured text into useful information.

For example, a company may receive thousands of customer reviews. By using text analysis, the company can find whether customers are happy or unhappy, what products are being discussed, and what common complaints are appearing.

Common uses of text analysis include:

Use Case

Meaning

Language detection

Identifying the language of the text

Key term extraction

Finding important words or phrases

Entity detection

Finding names of people, places, dates, and organizations

PII detection

Detecting sensitive information like phone numbers or addresses

Text classification

Categorizing text into classes

Sentiment analysis

Finding whether text is positive, negative, or neutral

Text summarization

Creating a short summary from a large text

Text analysis is challenging because human language is complex. The same word can have different meanings in different contexts. For example, the word banks can refer to financial institutions or the sides of a river. This is why NLP techniques are required to extract meaning from text. The provided module explains text analysis as an NLP subset used to extract meaning, structure, and insights from unstructured text.

## Tokenization

## Meaning of Tokenization

Tokenization is the first step in text analysis. It means breaking a sentence, paragraph, or document into smaller units called tokens.

Usually, tokens are words, but they can also be punctuation marks, subwords, or phrases.

## Example

Sentence:

## We choose to go to the moon

Tokens:

## We

choose

to

go

to

the

moon

Here, the sentence is broken into individual words. Each word is treated as a token.

## Importance of Tokenization

Tokenization is important because computers cannot directly understand full sentences. By breaking text into smaller tokens, we can count words, remove unnecessary words, find important terms, and prepare text for machine learning models.

## Text Preprocessing Techniques

Before applying machine learning or text analysis, text must be cleaned and prepared. This process is called text preprocessing, as shown in Figure 2.

Figure 2: Text preprocessing techniques such as tokenization, lowercasing, stopword removal, punctuation removal, stemming, lemmatization, spelling correction, and normalization.

## Text Normalization

Text normalization means converting text into a standard format.

It may include:

- Converting words to lowercase.

- Removing punctuation.

- Removing special characters.

- Removing extra spaces.

## Example

Original text:

## Artificial Intelligence is Powerful!

Normalized text:

## artificial intelligence is powerful

## Importance

Normalization helps reduce duplicate forms of the same word. For example, AI, ai, and Ai may be treated as different words unless they are normalized.

However, sometimes normalization may remove useful meaning. For example, Mr. Banks as a person and banks as financial institutions may need to be treated differently.

## Stop Word Removal

Stop words are common words that usually do not carry strong meaning.

Examples:

## the, is, am, are, a, an, it, of, and, to

## Example

Sentence:

## AI is transforming the world.

After stopword removal:

## AI transforming world

## Importance

Stopword removal helps reduce noise and keeps only meaningful words for analysis.

## N-Gram Extraction

An n-gram is a group of one or more words appearing together.

Type

Meaning

Example

Unigram

One word

artificial

Bigram

Two words

artificial intelligence

Trigram

Three words

natural language processing

##

## Importance

Sometimes a group of words has more meaning than individual words.

For example:

## artificial intelligence

natural language processing

machine learning

These phrases should be understood together rather than as separate words.

## Stemming

Stemming is the process of reducing words to their root form by cutting word endings.

## Example

## playing → play

played → play

player → play

Another example:

## powering, powered, powerful → power

## Limitation

Stemming may produce words that are not valid dictionary words.

Example:

## intelligence → intellig

So, stemming is fast but not always accurate.

## Lemmatization

Lemmatization also converts words into their base form, but it uses grammar and vocabulary rules.

## Example

## running → run

businesses → business

experiences → experience

## Difference between Stemming and Lemmatization

Stemming

Lemmatization

Cuts word endings

Uses grammar rules

Faster

More accurate

May produce invalid words

Produces valid dictionary words

Example: intelligence → intellig

Example: running → run

## Parts of Speech Tagging

Parts of Speech tagging, also called POS tagging, means identifying the grammatical category of each word.

Examples of POS tags:

POS

Meaning

Noun

Name of person, place, thing

Verb

Action word

Adjective

Describing word

Adverb

Modifies verb/adjective

Pronoun

Replaces noun

##

## Example

Sentence:

## AI improves business performance.

POS tagging:

## AI → Noun

improves → Verb

business → Noun

performance → Noun

POS tagging helps the computer understand the role of each word in a sentence.

## Statistical Text Analysis

After tokenization and preprocessing, statistical methods can be used to understand text.

## Frequency Analysis

Frequency analysis means counting how many times each word appears in a document.

## Example

Text:

## AI improves business. AI improves decision-making.

Frequency table:

Term

Frequency

AI

2

improves

2

business

1

decision-making

1

##

## Importance

Words that appear frequently often indicate the main topic of the document.

For example, if words like AI, business, customer, and decision appear many times, the document is probably about AI in business.

Frequency analysis is useful for identifying the most common words in a document, but it may not always show the most meaningful words because common words may appear in many documents.

## TF-IDF

TF-IDF stands for "Term Frequency-Inverse Document Frequency."

It is used to find important words in a document compared to a group of documents.

## Term Frequency

Term Frequency means how many times a word appears in a document.

Formula:

## TF = Number of times a term appears in a document

Example:

If the word "agent" appears 6 times, then:

## TF(agent) = 6

## Inverse Document Frequency

Inverse Document Frequency checks whether a word is common or rare across all documents.

Formula:

## IDF(t) = log(N / df(t))

Where:

Symbol

Meaning

N

Total number of documents

df(t)

Number of documents containing term t

If a word appears in every document, it is not very special. If it appears in only one document, it becomes more important.

## TF-IDF Formula

## TF-IDF = TF × IDF

A high TF-IDF score means the word is important in one document but not common in all documents.

## Example

Suppose there are two documents:

Document A talks about Copilot Studio.

Document B talks about Microsoft Foundry.

Common words like AI, Microsoft, and agent may appear in both documents. So, they are not useful for distinguishing the documents.

But words like:

## copilot

studio

declarative

may be important for Document A.

Words like:

## foundry

code

develop

may be important for Document B.

Therefore, TF-IDF helps identify the special terms of each document. The provided module explains that TF-IDF gives high importance to words that appear frequently in one document but rarely across other documents.

## Bag-of-Words Model

Bag-of-Words is a text representation technique. It represents text as a collection of word counts.

In this model, grammar and word order are ignored. Only the presence or frequency of words is considered.

## Example

Sentence 1:

## AI improves business

Sentence 2:

## AI improves learning

Vocabulary:

## AI, improves, business, learning

Bag-of-words representation:

Sentence

AI

improves

business

learning

Sentence 1

1

1

1

0

Sentence 2

1

1

0

1

##

## Importance

Bag-of-words is useful for machine learning tasks such as:

- Spam detection.

- Sentiment analysis.

- Topic classification.

- Document categorization.

## Example Use Case

In spam email detection, words like

## free

winner

lottery

miracle cure

lose weight fast

may appear more frequently in spam emails. A machine learning model can use these words to classify emails as spam or not spam.

## TextRank

TextRank is an unsupervised graph-based algorithm used for text summarization and keyword extraction.

It is inspired by Google’s PageRank algorithm.

## TextRank for Summarization

In TextRank, each sentence is treated as a node in a graph. Connections between sentences are called edges. These edges are based on similarity between sentences.

## Steps in TextRank

- Split the document into sentences.

- Treat each sentence as a node.

- Calculate similarity between sentences.

- Create edges between similar sentences.

- Rank the sentences.

- Select the highest-ranked sentences as the summary.

## Example Text

## Cloud computing provides on-demand access to computing resources.

Computing resources include servers, storage, and networking.

Azure is Microsoft's cloud computing platform.

Organizations use cloud platforms to reduce infrastructure costs.

Cloud computing enables scalability and flexibility.

Important sentences may be:

## Cloud computing provides on-demand access to computing resources.

Azure is Microsoft's cloud computing platform.

Cloud computing enables scalability and flexibility.

So, the summary becomes:

## Cloud computing provides on-demand access to computing resources.

Azure is Microsoft's cloud computing platform.

Cloud computing enables scalability and flexibility.

This is called extractive summarization because the summary is created by selecting original sentences from the document.

TextRank can also be used for keyword extraction, where words are treated as nodes and important words are selected as keywords.

## Semantic Language Models

Older NLP methods mainly used word counts and statistics. Modern NLP uses semantic language models.

Semantic models try to understand the meaning of words and sentences.

## Word Embeddings

Word embeddings represent words as vectors.

A vector is a list of numbers.

Example:

Word

Vector

dog

[0.8, 0.6, 0.1]

cat

[0.7, 0.5, 0.2]

tree

[0.2, 0.1, 0.9]

Words with similar meanings have similar vector directions.

For example:

## dog and cat

are more similar than:

## dog and tree

because dog and cat are both animals.

The uploaded module explains that embeddings are multi-valued arrays of numbers that encode semantic relationships between tokens.

## Cosine Similarity

Cosine similarity is used to measure similarity between two vectors.

Formula:

## cosine similarity = A · B / ||A|| × ||B||

Where:

Symbol

Meaning

A · B

Dot product of vectors

If cosine similarity is close to 1, the words are highly similar.

If it is close to 0, the words are not very similar.

## Example

The similarity between dog and cat may be high because both are animals.

The similarity between dog and tree may be low because they belong to different categories.

## Vector Arithmetic

Semantic models can also perform vector operations.

Example:

## dog + young = puppy

cat + young = kitten

This means the model understands the relationship between adult animals and young animals.

Another example:

## kitten - puppy + dog = cat

This shows analogy-based reasoning.

## Contextual Embeddings

Modern models such as GPT use contextual embeddings. This means the meaning of a word is understood based on its surrounding words.

Example:

## I deposited money in the bank.

Here, bank means financial institution.

## The children sat near the river bank.

Here, bank means side of a river.

Contextual embeddings help models understand the correct meaning based on context.

Code

# Install necessary libraries

!pip install transformers datasets torch

# Import required libraries

import pandas as pd

import torch

from transformers import AutoTokenizer, AutoModelForSequenceClassification, pipeline

from datasets import Dataset

# Load sample dataset (you can upload your CSV file in Colab later)

# Simulating a tweet dataset

data = {

"tweet": [

"I love AI! It's making life so much easier.",

"I hate traffic jams. They ruin my mood.",

"This new phone is amazing! Best purchase ever.",

"I am feeling neutral about today's meeting.",

"Why is the internet so slow? It's frustrating."

]

}

# Save the dataset as a CSV file

tweet_df = pd.DataFrame(data)

tweet_df.to_csv("tweets.csv", index=False)

print("Sample dataset created: tweets.csv")

# Load the dataset into a DataFrame

df = pd.read_csv("tweets.csv")

print("Loaded dataset:")

print(df)

# Load pre-trained BERT model and tokenizer

model_name = "distilbert-base-uncased-finetuned-sst-2-english"

tokenizer = AutoTokenizer.from_pretrained(model_name)

model = AutoModelForSequenceClassification.from_pretrained(model_name)

# Create a sentiment analysis pipeline

sentiment_pipeline = pipeline("sentiment-analysis", model=model, tokenizer=tokenizer)

# Perform sentiment analysis on the tweets

results = sentiment_pipeline(df["tweet"].tolist())

# Convert results to a DataFrame

results_df = pd.DataFrame(results)

df["label"] = results_df["label"]

df["score"] = results_df["score"]

# Display results

print("Sentiment Analysis Results:")

print(df)

# Save the results to a CSV file

df.to_csv("sentiment_analysis_results.csv", index=False)

print("Results saved to sentiment_analysis_results.csv")

# Visualize results

import seaborn as sns

import matplotlib.pyplot as plt

sns.countplot(data=df, x="label", palette="viridis")

plt.title("Sentiment Distribution")

plt.show()

##

##

## Practical Task Questions

- Write a Python program to perform tokenization on a given paragraph and display all tokens.

- Write a Python program to convert a given text into lowercase and remove all punctuation marks.

- Write a Python program to remove stop words from a given paragraph using the NLTK library.

- Write a Python program to perform stemming on the following words:

playing, played, player, studies, studying, powerful

- Write a Python program to perform lemmatization on a list of words and compare the output with stemming.

- Write a Python program to apply Part-of-Speech tagging to a sentence and identify nouns, verbs, and adjectives.

- Write a Python program to count the frequency of each word in a given text corpus.

- Write a Python program to create a Bag-of-Words model for three short documents.

- Write a Python program to calculate TF-IDF values for multiple text documents and display the important terms.

- Write a Python program to generate a simple extractive summary by selecting the most important sentences from a paragraph.

## Video Links

Basic Preprocessing—Case Folding, Stopword Removal, Stemming and Lemmatization

Natural Language Processing - Tokenization

Stemming and Lemmatization

Introduction to NLP | Bag of Words Model

Text Representation Using TF-IDF

## Additional Resources

- NLTK Official Documentation

URL: https://www.nltk.org/

Useful for tokenization, stemming, tagging, parsing, and text classification.

- NLTK Book — Natural Language Processing with Python

URL: https://www.nltk.org/book/

Useful for learning NLP basics with Python examples.

- Scikit-learn: Feature Extraction Documentation

URL: https://scikit-learn.org/stable/modules/feature_extraction.html

Useful for text feature extraction, Bag-of-Words, and TF-IDF.

- Scikit-learn: Working with Text Data

URL: https://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html

Useful for text classification and practical NLP pipelines.

- Scikit-learn: TfidfVectorizer Documentation

URL: https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html

Useful for converting text documents into TF-IDF feature matrices.

- GeeksforGeeks: Text Preprocessing in NLP

URL: https://www.geeksforgeeks.org/nlp/text-preprocessing-for-nlp-tasks/

Useful for tokenization, stopword removal, stemming, lemmatization, and POS tagging.

- Sanfoundry: Text Preprocessing in NLP

URL: https://www.sanfoundry.com/text-preprocessing-in-nlp-tokenization-stemming-lemmatization/

Useful for basic explanation and Python workflow of NLP preprocessing.

- RPI: Bag-of-Words Using Scikit-learn

URL: https://pages.github.rpi.edu/kuruzj/website_introml_rpi/notebooks/08-intro-nlp/03-scikit-learn-text.html

Useful for understanding Bag-of-Words with Scikit-learn.

- ResearchGate: An Interpretation of Lemmatization and Stemming in NLP

URL: https://www.researchgate.net/publication/348306833_An_Interpretation_of_Lemmatization_and_Stemming_in_Natural_Language_Processing

Useful for theoretical understanding of stemming and lemmatization.

- Dev.to: Complete Guide to NLP Text Preprocessing

URL: https://dev.to/themustaphatijani/the-complete-guide-to-nlp-text-preprocessing-tokenization-normalization-stemming-lemmatization-50ap

Useful for tokenization, normalization, stemming, and lemmatization examples.

## Textbooks

- Natural Language Processing with Python — Steven Bird, Ewan Klein, Edward Loper

URL: https://www.nltk.org/book/

- Speech and Language Processing, 3rd Edition — Daniel Jurafsky and James H. Martin

URL: https://web.stanford.edu/~jurafsky/slp3/

- Introduction to Information Retrieval — Christopher D. Manning, Prabhakar Raghavan, Hinrich Schütze

URL: https://nlp.stanford.edu/IR-book/pdf/irbookonlinereading.pdf

- Foundations of Statistical Natural Language Processing — Christopher D. Manning and Hinrich Schütze

URL: https://nlp.stanford.edu/fsnlp/

- Deep Learning for Natural Language Processing: A Gentle Introduction — Michael Roth, Mihai Surdeanu, and others

URL: https://clulab.org/gentlenlp/book/gentlenlp-book-12232022.pdf

## Reference Books

- A Primer on Neural Network Models for Natural Language Processing — Yoav Goldberg

URL: https://u.cs.biu.ac.il/~yogo/nnlp.pdf

- Neural Network Methods for Natural Language Processing — Yoav Goldberg

URL: https://link.springer.com/book/10.1007/978-3-031-02165-7

- Information Theory, Inference, and Learning Algorithms — David J. C. MacKay

URL: https://www.inference.org.uk/itprnn/book.pdf

- Taming Text: How to Find, Organize, and Manipulate It — Grant S. Ingersoll, Thomas S. Morton, Drew Farris

URL: https://www.manning.com/books/taming-text

- Introduction to Information Retrieval — Cambridge Book Information — Manning, Raghavan, Schütze

URL: https://assets.cambridge.org/97805218/65715/frontmatter/9780521865715_frontmatter.pdf